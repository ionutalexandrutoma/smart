<template>
  <PostSearch/>
</template>

<script>
import PostSearch from "./components/PostSearch.vue";

export default {
  name: 'App',
  components: {
    PostSearch
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.imgF{
  max-width: 2rem;
  margin: 0 5px;
}

.codeSource {
    transition: all 1s;
    cursor: normal;
}

.gist:hover{
  background-color: rgb(0 0 0 / 8%);
  cursor: pointer;
}

.lgueB p{
  color: #fff;
  text-shadow: 1px 1px 1px #6e6366;
  border-radius: 5px;
}

.ABAP{background-color: #E8274B;}
.ABAP CDS{background-color: #555e25;}
.ActionScript{background-color: #882B0F;}
.Ada{background-color: #02f88c;}
.Adblock Filter List{background-color: #800000;}
.Adobe Font Metrics{background-color: #fa0f00;}
.Agda{background-color: #315665;}
.AGS Script{background-color: #B9D9FF;}
.AIDL{background-color: #34EB6B;}
.AL{background-color: #3AA2B5;}
.Alloy{background-color: #64C800;}
.Alpine Abuild{background-color: #0D597F;}
.Altium Designer{background-color: #A89663;}
.AMPL{background-color: #E6EFBB;}
.AngelScript{background-color: #C7D7DC;}
.Ant Build System{background-color: #A9157E;}
.Antlers{background-color: #ff269e;}
.ANTLR{background-color: #9DC3FF;}
.ApacheConf{background-color: #d12127;}
.Apex{background-color: #1797c0;}
.API Blueprint{background-color: #2ACCA8;}
.APL{background-color: #5A8164;}
.Apollo Guidance Computer{background-color: #0B3D91;}
.AppleScript{background-color: #101F1F;}
.Arc{background-color: #aa2afe;}
.AsciiDoc{background-color: #73a0c5;}
.ASP.NET{background-color: #9400ff;}
.AspectJ{background-color: #a957b0;}
.Assembly{background-color: #6E4C13;}
.Astro{background-color: #ff5a03;}
.Asymptote{background-color: #ff0000;}
.ATS{background-color: #1ac620;}
.Augeas{background-color: #9CC134;}
.AutoHotkey{background-color: #6594b9;}
.AutoIt{background-color: #1C3552;}
.Avro IDL{background-color: #0040FF;}
.Awk{background-color: #c30e9b;}
.Ballerina{background-color: #FF5000;}
.BASIC{background-color: #ff0000;}
.Batchfile{background-color: #C1F12E;}
.Beef{background-color: #a52f4e;}
.Berry{background-color: #15A13C;}
.BibTeX{background-color: #778899;}
.Bicep{background-color: #519aba;}
.Bikeshed{background-color: #5562ac;}
.Bison{background-color: #6A463F;}
.BitBake{background-color: #00bce4;}
.Blade{background-color: #f7523f;}
.BlitzBasic{background-color: #00FFAE;}
.BlitzMax{background-color: #cd6400;}
.Bluespec{background-color: #12223c;}
.Boo{background-color: #d4bec1;}
.Boogie{background-color: #c80fa0;}
.Brainfuck{background-color: #2F2530;}
.BrighterScript{background-color: #66AABB;}
.Brightscript{background-color: #662D91;}
.Browserslist{background-color: #ffd539;}
.C{background-color: #555555;}
.C#{background-color: #178600;}
.C++{background-color: #f34b7d;}
.Cabal Config{background-color: #483465;}
.Cadence{background-color: #00ef8b;}
.Cairo{background-color: #ff4a48;}
.CameLIGO{background-color: #3be133;}
.CAP CDS{background-color: #0092d1;}
.Cap\'n Proto{background-color: #c42727;}
.Ceylon{background-color: #dfa535;}
.Chapel{background-color: #8dc63f;}
.ChucK{background-color: #3f8000;}
.Cirru{background-color: #ccccff;}
.Clarion{background-color: #db901e;}
.Clarity{background-color: #5546ff;}
.Classic ASP{background-color: #6a40fd;}
.Clean{background-color: #3F85AF;}
.Click{background-color: #E4E6F3;}
.CLIPS{background-color: #00A300;}
.Clojure{background-color: #db5855;}
.Closure Templates{background-color: #0d948f;}
.Cloud Firestore Security Rules{background-color: #FFA000;}
.CMake{background-color: #DA3434;}
.CodeQL{background-color: #140f46;}
.CoffeeScript{background-color: #244776;}
.ColdFusion{background-color: #ed2cd6;}
.ColdFusion CFC{background-color: #ed2cd6;}
.COLLADA{background-color: #F1A42B;}
.Common Lisp{background-color: #3fb68b;}
.Common Workflow Language{background-color: #B5314C;}
.Component Pascal{background-color: #B0CE4E;}
.Coq{background-color: #d0b68c;}
.Crystal{background-color: #000100;}
.CSON{background-color: #244776;}
.Csound{background-color: #1a1a1a;}
.Csound Document{background-color: #1a1a1a;}
.Csound Score{background-color: #1a1a1a;}
.CSS{background-color: #563d7c;}
.CSV{background-color: #237346;}
.Cuda{background-color: #3A4E3A;}
.CUE{background-color: #5886E1;}
.Curry{background-color: #531242;}
.CWeb{background-color: #00007a;}
.Cypher{background-color: #34c0eb;}
.Cython{background-color: #fedf5b;}
.D{background-color: #ba595e;}
.Dafny{background-color: #FFEC25;}
.Darcs Patch{background-color: #8eff23;}
.Dart{background-color: #00B4AB;}
.DataWeave{background-color: #003a52;}
.Debian Package Control File{background-color: #D70751;}
.DenizenScript{background-color: #FBEE96;}
.Dhall{background-color: #dfafff;}
.DirectX3DFile{background-color: #aace60;}
.DM{background-color: #447265;}
.Dockerfile{background-color: #384d54;}
.Dogescript{background-color: #cca760;}
.Dylan{background-color: #6c616e;}
.E{background-color: #ccce35;}
.Earthly{background-color: #2af0ff;}
.Easybuild{background-color: #069406;}
.eC{background-color: #913960;}
.Ecere Projects{background-color: #913960;}
.ECL{background-color: #8a1267;}
.ECLiPSe{background-color: #001d9d;}
.Ecmarkup{background-color: #eb8131;}
.EditorConfig{background-color: #fff1f2;}
.Eiffel{background-color: #4d6977;}
.EJS{background-color: #a91e50;}
.Elixir{background-color: #6e4a7e;}
.Elm{background-color: #60B5CC;}
.Elvish{background-color: #55BB55;}
.Emacs Lisp{background-color: #c065db;}
.EmberScript{background-color: #FFF4F3;}
.EQ{background-color: #a78649;}
.Erlang{background-color: #B83998;}
.Euphoria{background-color: #FF790B;}
.Factor{background-color: #636746;}
.Fancy{background-color: #7b9db4;}
.Fantom{background-color: #14253c;}
.Faust{background-color: #c37240;}
.Fennel{background-color: #fff3d7;}
.FIGlet Font{background-color: #FFDDBB;}
.Filebench WML{background-color: #F6B900;}
.fish{background-color: #4aae47;}
.Fluent{background-color: #ffcc33;}
.FLUX{background-color: #88ccff;}
.Forth{background-color: #341708;}
.Fortran{background-color: #4d41b1;}
.Fortran Free Form{background-color: #4d41b1;}
.FreeBasic{background-color: #867db1;}
.FreeMarker{background-color: #0050b2;}
.Frege{background-color: #00cafe;}
.Futhark{background-color: #5f021f;}
.G-code{background-color: #D08CF2;}
.Game Maker Language{background-color: #71b417;}
.GAML{background-color: #FFC766;}
.GAMS{background-color: #f49a22;}
.GAP{background-color: #0000cc;}
.GCC Machine Description{background-color: #FFCFAB;}
.GDScript{background-color: #355570;}
.GEDCOM{background-color: #003058;}
.Gemfile.lock{background-color: #701516;}
.Gemini{background-color: #ff6900;}
.Genero{background-color: #63408e;}
.Genero Forms{background-color: #d8df39;}
.Genie{background-color: #fb855d;}
.Genshi{background-color: #951531;}
.Gentoo Ebuild{background-color: #9400ff;}
.Gentoo Eclass{background-color: #9400ff;}
.Gerber Image{background-color: #d20b00;}
.Gherkin{background-color: #5B2063;}
.Git Attributes{background-color: #F44D27;}
.Git Config{background-color: #F44D27;}
.Git Revision List{background-color: #F44D27;}
.Gleam{background-color: #ffaff3;}
.GLSL{background-color: #5686a5;}
.Glyph{background-color: #c1ac7f;}
.Gnuplot{background-color: #f0a9f0;}
.Go{background-color: #00ADD8;}
.Go Checksums{background-color: #00ADD8;}
.Go Module{background-color: #00ADD8;}
.Golo{background-color: #88562A;}
.Gosu{background-color: #82937f;}
.Grace{background-color: #615f8b;}
.Gradle{background-color: #02303a;}
.Grammatical Framework{background-color: #ff0000;}
.GraphQL{background-color: #e10098;}
.GraphvizDOT{background-color: #2596be;}
.Groovy{background-color: #4298b8;}
.Groovy Server Pages{background-color: #4298b8;}
.GSC{background-color: #FF6800;}
.Hack{background-color: #878787;}
.Haml{background-color: #ece2a9;}
.Handlebars{background-color: #f7931e;}
.HAProxy{background-color: #106da9;}
.Harbour{background-color: #0e60e3;}
.Haskell{background-color: #5e5086;}
.Haxe{background-color: #df7900;}
.HiveQL{background-color: #dce200;}
.HLSL{background-color: #aace60;}
.HOCON{background-color: #9ff8ee;}
.HolyC{background-color: #ffefaf;}
.hoon{background-color: #00b171;}
.HTML{background-color: #e34c26;}
.HTML+ECR{background-color: #2e1052;}
.HTML+EEX{background-color: #6e4a7e;}
.HTML+ERB{background-color: #701516;}
.HTML+PHP{background-color: #4f5d95;}
.HTML+Razor{background-color: #512be4;}
.HTTP{background-color: #005C9C;}
.HXML{background-color: #f68712;}
.Hy{background-color: #7790B2;}
.IDL{background-color: #a3522f;}
.Idris{background-color: #b30000;}
.Ignore List{background-color: #000000;}
.IGOR Pro{background-color: #0000cc;}
.ImageJ Macro{background-color: #99AAFF;}
.Imba{background-color: #16cec6;}
.INI{background-color: #d1dbe0;}
.Inno Setup{background-color: #264b99;}
.Io{background-color: #a9188d;}
.Ioke{background-color: #078193;}
.Isabelle{background-color: #FEFE00;}
.Isabelle ROOT{background-color: #FEFE00;}
.J{background-color: #9EEDFF;}
.Janet{background-color: #0886a5;}
.JAR Manifest{background-color: #b07219;}
.Jasmin{background-color: #d03600;}
.Java{background-color: #b07219;}
.Java Properties{background-color: #2A6277;}
.Java Server Pages{background-color: #2A6277;}
.JavaScript{background-color: #f1e05a;}
.JavaScript+ERB{background-color: #f1e05a;}
.Jest Snapshot{background-color: #15c213;}
.JetBrains MPS{background-color: #21D789;}
.JFlex{background-color: #DBCA00;}
.Jinja{background-color: #a52a22;}
.Jison{background-color: #56b3cb;}
.Jison Lex{background-color: #56b3cb;}
.Jolie{background-color: #843179;}
.jq{background-color: #c7254e;}
.JSON{background-color: #292929;}
.JSON with Comments{background-color: #292929;}
.JSON5{background-color: #267CB9;}
.JSONiq{background-color: #40d47e;}
.JSONLD{background-color: #0c479c;}
.Jsonnet{background-color: #0064bd;}
.Julia{background-color: #a270ba;}
.Jupyter Notebook{background-color: #DA5B0B;}
.just{background-color: #384d54;}
.Kaitai Struct{background-color: #773b37;}
.KakouneScript{background-color: #6f8042;}
.KiCad Layout{background-color: #2f4aab;}
.KiCad Legacy Layout{background-color: #2f4aab;}
.KiCad Schematic{background-color: #2f4aab;}
.Kotlin{background-color: #A97BFF;}
.KRL{background-color: #28430A;}
.kvlang{background-color: #1da6e0;}
.LabVIEW{background-color: #fede06;}
.Lark{background-color: #2980B9;}
.Lasso{background-color: #999999;}
.Latte{background-color: #f2a542;}
.Less{background-color: #1d365d;}
.Lex{background-color: #DBCA00;}
.LFE{background-color: #4C3023;}
.LigoLANG{background-color: #0e74ff;}
.LilyPond{background-color: #9ccc7c;}
.Liquid{background-color: #67b8de;}
.Literate Agda{background-color: #315665;}
.Literate CoffeeScript{background-color: #244776;}
.Literate Haskell{background-color: #5e5086;}
.LiveScript{background-color: #499886;}
.LLVM{background-color: #185619;}
.Logtalk{background-color: #295b9a;}
.LOLCODE{background-color: #cc9900;}
.LookML{background-color: #652B81;}
.LSL{background-color: #3d9970;}
.Lua{background-color: #000080;}
.Macaulay2{background-color: #d8ffff;}
.Makefile{background-color: #427819;}
.Mako{background-color: #7e858d;}
.Markdown{background-color: #083fa1;}
.Marko{background-color: #42bff2;}
.Mask{background-color: #f97732;}
.Mathematica{background-color: #dd1100;}
.MATLAB{background-color: #e16737;}
.Max{background-color: #c4a79c;}
.MAXScript{background-color: #00a6a6;}
.mcfunction{background-color: #E22837;}
.Mercury{background-color: #ff2b2b;}
.Mermaid{background-color: #ff3670;}
.Meson{background-color: #007800;}
.Metal{background-color: #8f14e9;}
.MiniYAML{background-color: #ff1111;}
.Mint{background-color: #02b046;}
.Mirah{background-color: #c7a938;}
.mIRC Script{background-color: #3d57c3;}
.MLIR{background-color: #5EC8DB;}
.Modelica{background-color: #de1d31;}
.Modula-2{background-color: #10253f;}
.Modula-3{background-color: #223388;}
.Monkey C{background-color: #8D6747;}
.MoonScript{background-color: #ff4585;}
.Motoko{background-color: #fbb03b;}
.Motorola68KAssembly{background-color: #005daa;}
.Move{background-color: #4a137a;}
.MQL4{background-color: #62A8D6;}
.MQL5{background-color: #4A76B8;}
.MTML{background-color: #b7e1f4;}
.mupad{background-color: #244963;}
.Mustache{background-color: #724b3b;}
.nanorc{background-color: #2d004d;}
.Nasal{background-color: #1d2c4e;}
.NCL{background-color: #28431f;}
.Nearley{background-color: #990000;}
.Nemerle{background-color: #3d3c6e;}
.nesC{background-color: #94B0C7;}
.NetLinx{background-color: #0aa0ff;}
.NetLinx+ERB{background-color: #747faa;}
.NetLogo{background-color: #ff6375;}
.NewLisp{background-color: #87AED7;}
.Nextflow{background-color: #3ac486;}
.Nginx{background-color: #009639;}
.Nim{background-color: #ffc200;}
.Nit{background-color: #009917;}
.Nix{background-color: #7e7eff;}
.NPM Config{background-color: #cb3837;}
.Nu{background-color: #c9df40;}
.NumPy{background-color: #9C8AF9;}
.Nunjucks{background-color: #3d8137;}
.NWScript{background-color: #111522;}
.OASv2-json{background-color: #85ea2d;}
.OASv2-yaml{background-color: #85ea2d;}
.OASv3-json{background-color: #85ea2d;}
.OASv3-yaml{background-color: #85ea2d;}
.Objective-C{background-color: #438eff;}
.Objective-C++{background-color: #6866fb;}
.Objective-J{background-color: #ff0c5a;}
.ObjectScript{background-color: #424893;}
.OCaml{background-color: #3be133;}
.Odin{background-color: #60AFFE;}
.Omgrofl{background-color: #cabbff;}
.ooc{background-color: #b0b77e;}
.Opal{background-color: #f7ede0;}
.Open Policy Agent{background-color: #7d9199;}
.OpenAPI Specification v2{background-color: #85ea2d;}
.OpenAPI Specification v3{background-color: #85ea2d;}
.OpenCL{background-color: #ed2e2d;}
.OpenEdge ABL{background-color: #5ce600;}
.OpenQASM{background-color: #AA70FF;}
.OpenSCAD{background-color: #e5cd45;}
.Option List{background-color: #476732;}
.Org{background-color: #77aa99;}
.Oxygene{background-color: #cdd0e3;}
.Oz{background-color: #fab738;}
.P4{background-color: #7055b5;}
.Pan{background-color: #cc0000;}
.Papyrus{background-color: #6600cc;}
.Parrot{background-color: #f3ca0a;}
.Pascal{background-color: #E3F171;}
.Pawn{background-color: #dbb284;}
.PDDL{background-color: #0d00ff;}
.PEG.js{background-color: #234d6b;}
.Pep8{background-color: #C76F5B;}
.Perl{background-color: #0298c3;}
.PHP{background-color: #4F5D95;}
.PicoLisp{background-color: #6067af;}
.PigLatin{background-color: #fcd7de;}
.Pike{background-color: #005390;}
.PLpgSQL{background-color: #336790;}
.PLSQL{background-color: #dad8d8;}
.PogoScript{background-color: #d80074;}
.Polar{background-color: #ae81ff;}
.Portugol{background-color: #f8bd00;}
.PostCSS{background-color: #dc3a0c;}
.PostScript{background-color: #da291c;}
.POV-Ray SDL{background-color: #6bac65;}
.PowerBuilder{background-color: #8f0f8d;}
.PowerShell{background-color: #012456;}
.Prisma{background-color: #0c344b;}
.Processing{background-color: #0096D8;}
.Procfile{background-color: #3B2F63;}
.Prolog{background-color: #74283c;}
.Promela{background-color: #de0000;}
.Propeller Spin{background-color: #7fa2a7;}
.Pug{background-color: #a86454;}
.Puppet{background-color: #302B6D;}
.PureBasic{background-color: #5a6986;}
.PureScript{background-color: #1D222D;}
.Python{background-color: #3572A5;}
.Python console{background-color: #3572A5;}
.Python traceback{background-color: #3572A5;}
.q{background-color: #0040cd;}
.Q#{background-color: #fed659;}
.QML{background-color: #44a51c;}
.Qt Script{background-color: #00b841;}
.Quake{background-color: #882233;}
.R{background-color: #198CE7;}
.Racket{background-color: #3c5caa;}
.Ragel{background-color: #9d5200;}
.Raku{background-color: #0000fb;}
.RAML{background-color: #77d9fb;}
.Rascal{background-color: #fffaa0;}
.RDoc{background-color: #701516;}
.Reason{background-color: #ff5847;}
.ReasonLIGO{background-color: #ff5847;}
.Rebol{background-color: #358a5b;}
.Record Jar{background-color: #0673ba;}
.Red{background-color: #f50000;}
.Regular Expression{background-color: #009a00;}
.Ren\'Py{background-color: #ff7f7f;}
.ReScript{background-color: #ed5051;}
.reStructuredText{background-color: #141414;}
.REXX{background-color: #d90e09;}
.Ring{background-color: #2D54CB;}
.Riot{background-color: #A71E49;}
.RMarkdown{background-color: #198ce7;}
.RobotFramework{background-color: #00c0b5;}
.Roff{background-color: #ecdebe;}
.Roff Manpage{background-color: #ecdebe;}
.Rouge{background-color: #cc0088;}
.RouterOS Script{background-color: #DE3941;}
.RPGLE{background-color: #2BDE21;}
.Ruby{background-color: #701516;}
.RUNOFF{background-color: #665a4e;}
.Rust{background-color: #dea584;}
.SaltStack{background-color: #646464;}
.SAS{background-color: #B34936;}
.Sass{background-color: #a53b70;}
.Scala{background-color: #c22d40;}
.Scaml{background-color: #bd181a;}
.Scenic{background-color: #fdc700;}
.Scheme{background-color: #1e4aec;}
.Scilab{background-color: #ca0f21;}
.SCSS{background-color: #c6538c;}
.sed{background-color: #64b970;}
.Self{background-color: #0579aa;}
.ShaderLab{background-color: #222c37;}
.Shell{background-color: #89e051;}
.ShellCheck Config{background-color: #cecfcb;}
.Shen{background-color: #120F14;}
.Simple File Verification{background-color: #C9BFED;}
.Singularity{background-color: #64E6AD;}
.Slash{background-color: #007eff;}
.Slice{background-color: #003fa2;}
.Slim{background-color: #2b2b2b;}
.Smalltalk{background-color: #596706;}
.Smarty{background-color: #f0c040;}
.Smithy{background-color: #c44536;}
.SmPL{background-color: #c94949;}
.Solidity{background-color: #AA6746;}
.SourcePawn{background-color: #f69e1d;}
.SPARQL{background-color: #0C4597;}
.SQF{background-color: #3F3F3F;}
.SQL{background-color: #e38c00;}
.SQLPL{background-color: #e38c00;}
.Squirrel{background-color: #800000;}
.SRecode Template{background-color: #348a34;}
.Stan{background-color: #b2011d;}
.Standard ML{background-color: #dc566d;}
.Starlark{background-color: #76d275;}
.Stata{background-color: #1a5f91;}
.STL{background-color: #373b5e;}
.StringTemplate{background-color: #3fb34f;}
.Stylus{background-color: #ff6347;}
.SubRip Text{background-color: #9e0101;}
.SugarSS{background-color: #2fcc9f;}
.SuperCollider{background-color: #46390b;}
.Svelte{background-color: #ff3e00;}
.SVG{background-color: #ff9900;}
.Swift{background-color: #F05138;}
.SystemVerilog{background-color: #DAE1C2;}
.Talon{background-color: #333333;}
.Tcl{background-color: #e4cc98;}
.Terra{background-color: #00004c;}
.TeX{background-color: #3D6117;}
.Textile{background-color: #ffe7ac;}
.TextMate Properties{background-color: #df66e4;}
.Thrift{background-color: #D12127;}
.TI Program{background-color: #A0AA87;}
.TLA{background-color: #4b0079;}
.TOML{background-color: #9c4221;}
.TSQL{background-color: #e38c00;}
.TSV{background-color: #237346;}
.TSX{background-color: #3178c6;}
.Turing{background-color: #cf142b;}
.Twig{background-color: #c1d026;}
.TXL{background-color: #0178b8;}
.TypeScript{background-color: #3178c6;}
.Unified Parallel C{background-color: #4e3617;}
.Unity3D Asset{background-color: #222c37;}
.Uno{background-color: #9933cc;}
.UnrealScript{background-color: #a54c4d;}
.UrWeb{background-color: #ccccee;}
.V{background-color: #4f87c4;}
.Vala{background-color: #a56de2;}
.Valve Data Format{background-color: #f26025;}
.VBA{background-color: #867db1;}
.VBScript{background-color: #15dcdc;}
.VCL{background-color: #148AA8;}
.Velocity Template Language{background-color: #507cff;}
.Verilog{background-color: #b2b7f8;}
.VHDL{background-color: #adb2cb;}
.Vim Help File{background-color: #199f4b;}
.Vim Script{background-color: #199f4b;}
.Vim Snippet{background-color: #199f4b;}
.Visual Basic .NET{background-color: #945db7;}
.Visual Basic 6.0{background-color: #2c6353;}
.Volt{background-color: #1F1F1F;}
.Vue{background-color: #41b883;}
.Vyper{background-color: #2980b9;}
.wdl{background-color: #42f1f4;}
.Web Ontology Language{background-color: #5b70bd;}
.WebAssembly{background-color: #04133b;}
.Whiley{background-color: #d5c397;}
.Wikitext{background-color: #fc5757;}
.Windows Registry Entries{background-color: #52d5ff;}
.wisp{background-color: #7582D1;}
.Witcher Script{background-color: #ff0000;}
.Wollok{background-color: #a23738;}
.World of Warcraft Addon Data{background-color: #f7e43f;}
.Wren{background-color: #383838;}
.X10{background-color: #4B6BEF;}
.xBase{background-color: #403a40;}
.XC{background-color: #99DA07;}
.XML{background-color: #0060ac;}
.XML Property List{background-color: #0060ac;}
.Xojo{background-color: #81bd41;}
.Xonsh{background-color: #285EEF;}
.XQuery{background-color: #5232e7;}
.XSLT{background-color: #EB8CEB;}
.Xtend{background-color: #24255d;}
.Yacc{background-color: #4B6C4B;}
.YAML{background-color: #cb171e;}
.YARA{background-color: #220000;}
.YASnippet{background-color: #32AB90;}
.Yul{background-color: #794932;}
.ZAP{background-color: #0d665e;}
.ZenScript{background-color: #00BCD1;}
.Zephir{background-color: #118f9e;}
.Zig{background-color: #ec915c;}
.ZIL{background-color: #dc75e5;}
.Zimpl{background-color: #d67711;}
</style>
