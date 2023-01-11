<template>
    <nav class="navbar navbar-expand-lg bg-light">
      <div class="container-fluid">
        <form class="d-flex ms-auto me-auto p-3 needs-validation" id="search_frm" role="search" novalidate @submit.prevent="getData" method="get">
            <input class="form-control me-2" id="search_i" type="search" placeholder="Search user" aria-label="Search" v-model="user">
            <button class="btn btn-outline-success" type="submit"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
            <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
            </svg></button>
        </form>
        </div>
    </nav>      
    <div class="container">
        <div v-if="err" class="row justify-content-center text-center">
            <h3 class="mt-3">User not found!</h3>
        </div>
        <div v-else-if="loading" class="row justify-content-center text-center">
            <div class="spinner-border mt-3" role="status">
                <span class="visually-hidden">Loading...</span>
            </div>
        </div>
        <div v-else-if="data && !err" class="row justify-content-center text-center">
            <div class="col-md-3">
                <img :src="data.user.avatar_url" class="rounded-circle mx-auto d-block w-100 p-3"/>
                <h4 class="mb-0"><b>{{ data.user.name }}</b></h4>
                <p class="text-gray mb-0">{{ data.user.login }}</p>
                <p class="mb-0"><b>{{ data.user.bio }}</b></p>
            </div>
            <div class="col-md-9">
                <div v-for="gist in data.gists" :key="gist.id">
                    <div v-for="file in gist.files" :key="file.filename">
                        <div class="row justify-content-center pt-2 pb-2 border-bottom gist" @click="showCode(file.raw_url, gist.id + file.filename)" :id="gist.id + file.filename">
                            <div class="col-4 col-md-2 col-lg-1">
                                <img :src="gist.owner.avatar_url" class="rounded-circle mx-auto d-block w-100 p-1"/>
                            </div>
                            <div class="col-12 col-md-7 col-lg-9 text-center text-md-start">
                                <span class="text-primary"><b>{{ gist.owner.login }}</b> </span> / <span class="text-primary"><b>{{ file.filename }}</b> </span> <br>
                                <span class="text-gray"><small> Created at: {{ gist.created_at }} </small></span>
                            </div>
                            <div class="col-md-3 col-lg-2 my-auto">
                                <div class="rounded p-2 lgueB">
                                    <p :class="file.language"> {{ file.language }} </p>
                                </div>
                            </div>
                            <div v-if="gist.forksDet" class="col-12 text-start">
                                <p class="d-inline">Forked by:</p>
                                <div v-for="fork in gist.forksDet.slice(0, 3)" :key="fork.id" class="d-inline">
                                    <img :src="fork.owner.avatar_url" class="rounded-circle d-inline imgF"/>
                                    <p class="d-inline">{{ fork.owner.login }} </p>
                                </div>
                                <p v-if="gist.forksDet.length > 3" class="d-inline"> and more others.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div> 
        </div>
        <div v-else>
            <h3 class="mt-3">Your results will be here...</h3>
        </div>
    </div>
</template>
  
<script>
    import $ from 'jquery'
    import { Octokit } from "@octokit/rest"

    export default {
        name: 'PostSearch',
        data(){
            return {
                user: null,
                data: null,
                err: null,
                loading: null
            }
        },
        methods:{
            async getData(e){
                this.err = null
                this.loading = true
                const octokit = new Octokit({
                    auth: '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'
                })

                const resultUser = await octokit.request('GET /users/' + this.user, {
                    username: this.user
                }).catch(e => {
                    this.err = e
                })

                const userObj = {}
                const frks = {}

                if(this.user === null)
                    this.err = "Not found!"

                if(!this.err && resultUser.data.id){
                    userObj.user = resultUser.data

                    const resultGists = await octokit.request('GET /users/' + this.user + '/gists{?since,per_page,page}', {
                        username: this.user
                    }) 

                    for( const gist of resultGists.data ){
                        gist.created_at = gist.created_at.replace("T", " ").replace("Z", " ")
                        if(gist.forks_url.length){
                            
                            await $.getJSON(gist.forks_url,function(forks){
                                if(forks.length)
                                    gist.forksDet = forks
                            })
                        }
                    }
                    
                    userObj.gists = resultGists.data
                }
                else{
                    this.err = "Not found!"
                }  
                
                this.frks = frks
                console.log(userObj);
                this.data = userObj
                this.loading = false

                e.preventDefault()
            },
            async showCode(url, el_id){
                var div = document.getElementById(el_id)

                const boxes = document.querySelectorAll('.codeSourceCnt')
                
                boxes.forEach(box => {
                    box.remove()
                })

                await $.get(url,function(text){
                    if(text.length){   
                        div.outerHTML += '<div class="row codeSourceCnt"><div class="col-12 p-3 bg-dark text-white"><div class="codeSource text-start"><pre><code>' + text + '</pre></code></div></div></div>'
                    }
                })

                return
            }
        }
    }
</script>
  