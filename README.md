<!DOCTYPE html><html><head>
      <title>WJR_UCB_Exchange</title>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      
      <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.css">
      
      

      
      
      
      
      
      
      

      <style>
      /**
 * prism.js Github theme based on GitHub's theme.
 * @author Sam Clarke
 */
code[class*="language-"],
pre[class*="language-"] {
  color: #333;
  background: none;
  font-family: Consolas, "Liberation Mono", Menlo, Courier, monospace;
  text-align: left;
  white-space: pre;
  word-spacing: normal;
  word-break: normal;
  word-wrap: normal;
  line-height: 1.4;

  -moz-tab-size: 8;
  -o-tab-size: 8;
  tab-size: 8;

  -webkit-hyphens: none;
  -moz-hyphens: none;
  -ms-hyphens: none;
  hyphens: none;
}

/* Code blocks */
pre[class*="language-"] {
  padding: .8em;
  overflow: auto;
  /* border: 1px solid #ddd; */
  border-radius: 3px;
  /* background: #fff; */
  background: #f5f5f5;
}

/* Inline code */
:not(pre) > code[class*="language-"] {
  padding: .1em;
  border-radius: .3em;
  white-space: normal;
  background: #f5f5f5;
}

.token.comment,
.token.blockquote {
  color: #969896;
}

.token.cdata {
  color: #183691;
}

.token.doctype,
.token.punctuation,
.token.variable,
.token.macro.property {
  color: #333;
}

.token.operator,
.token.important,
.token.keyword,
.token.rule,
.token.builtin {
  color: #a71d5d;
}

.token.string,
.token.url,
.token.regex,
.token.attr-value {
  color: #183691;
}

.token.property,
.token.number,
.token.boolean,
.token.entity,
.token.atrule,
.token.constant,
.token.symbol,
.token.command,
.token.code {
  color: #0086b3;
}

.token.tag,
.token.selector,
.token.prolog {
  color: #63a35c;
}

.token.function,
.token.namespace,
.token.pseudo-element,
.token.class,
.token.class-name,
.token.pseudo-class,
.token.id,
.token.url-reference .token.variable,
.token.attr-name {
  color: #795da3;
}

.token.entity {
  cursor: help;
}

.token.title,
.token.title .token.punctuation {
  font-weight: bold;
  color: #1d3e81;
}

.token.list {
  color: #ed6a43;
}

.token.inserted {
  background-color: #eaffea;
  color: #55a532;
}

.token.deleted {
  background-color: #ffecec;
  color: #bd2c00;
}

.token.bold {
  font-weight: bold;
}

.token.italic {
  font-style: italic;
}


/* JSON */
.language-json .token.property {
  color: #183691;
}

.language-markup .token.tag .token.punctuation {
  color: #333;
}

/* CSS */
code.language-css,
.language-css .token.function {
  color: #0086b3;
}

/* YAML */
.language-yaml .token.atrule {
  color: #63a35c;
}

code.language-yaml {
  color: #183691;
}

/* Ruby */
.language-ruby .token.function {
  color: #333;
}

/* Markdown */
.language-markdown .token.url {
  color: #795da3;
}

/* Makefile */
.language-makefile .token.symbol {
  color: #795da3;
}

.language-makefile .token.variable {
  color: #183691;
}

.language-makefile .token.builtin {
  color: #0086b3;
}

/* Bash */
.language-bash .token.keyword {
  color: #0086b3;
}

/* highlight */
pre[data-line] {
  position: relative;
  padding: 1em 0 1em 3em;
}
pre[data-line] .line-highlight-wrapper {
  position: absolute;
  top: 0;
  left: 0;
  background-color: transparent;
  display: block;
  width: 100%;
}

pre[data-line] .line-highlight {
  position: absolute;
  left: 0;
  right: 0;
  padding: inherit 0;
  margin-top: 1em;
  background: hsla(24, 20%, 50%,.08);
  background: linear-gradient(to right, hsla(24, 20%, 50%,.1) 70%, hsla(24, 20%, 50%,0));
  pointer-events: none;
  line-height: inherit;
  white-space: pre;
}

pre[data-line] .line-highlight:before, 
pre[data-line] .line-highlight[data-end]:after {
  content: attr(data-start);
  position: absolute;
  top: .4em;
  left: .6em;
  min-width: 1em;
  padding: 0 .5em;
  background-color: hsla(24, 20%, 50%,.4);
  color: hsl(24, 20%, 95%);
  font: bold 65%/1.5 sans-serif;
  text-align: center;
  vertical-align: .3em;
  border-radius: 999px;
  text-shadow: none;
  box-shadow: 0 1px white;
}

pre[data-line] .line-highlight[data-end]:after {
  content: attr(data-end);
  top: auto;
  bottom: .4em;
}html body{font-family:"Helvetica Neue",Helvetica,"Segoe UI",Arial,freesans,sans-serif;font-size:16px;line-height:1.6;color:#333;background-color:#fff;overflow:initial;box-sizing:border-box;word-wrap:break-word}html body>:first-child{margin-top:0}html body h1,html body h2,html body h3,html body h4,html body h5,html body h6{line-height:1.2;margin-top:1em;margin-bottom:16px;color:#000}html body h1{font-size:2.25em;font-weight:300;padding-bottom:.3em}html body h2{font-size:1.75em;font-weight:400;padding-bottom:.3em}html body h3{font-size:1.5em;font-weight:500}html body h4{font-size:1.25em;font-weight:600}html body h5{font-size:1.1em;font-weight:600}html body h6{font-size:1em;font-weight:600}html body h1,html body h2,html body h3,html body h4,html body h5{font-weight:600}html body h5{font-size:1em}html body h6{color:#5c5c5c}html body strong{color:#000}html body del{color:#5c5c5c}html body a:not([href]){color:inherit;text-decoration:none}html body a{color:#08c;text-decoration:none}html body a:hover{color:#00a3f5;text-decoration:none}html body img{max-width:100%}html body>p{margin-top:0;margin-bottom:16px;word-wrap:break-word}html body>ul,html body>ol{margin-bottom:16px}html body ul,html body ol{padding-left:2em}html body ul.no-list,html body ol.no-list{padding:0;list-style-type:none}html body ul ul,html body ul ol,html body ol ol,html body ol ul{margin-top:0;margin-bottom:0}html body li{margin-bottom:0}html body li.task-list-item{list-style:none}html body li>p{margin-top:0;margin-bottom:0}html body .task-list-item-checkbox{margin:0 .2em .25em -1.8em;vertical-align:middle}html body .task-list-item-checkbox:hover{cursor:pointer}html body blockquote{margin:16px 0;font-size:inherit;padding:0 15px;color:#5c5c5c;border-left:4px solid #d6d6d6}html body blockquote>:first-child{margin-top:0}html body blockquote>:last-child{margin-bottom:0}html body hr{height:4px;margin:32px 0;background-color:#d6d6d6;border:0 none}html body table{margin:10px 0 15px 0;border-collapse:collapse;border-spacing:0;display:block;width:100%;overflow:auto;word-break:normal;word-break:keep-all}html body table th{font-weight:bold;color:#000}html body table td,html body table th{border:1px solid #d6d6d6;padding:6px 13px}html body dl{padding:0}html body dl dt{padding:0;margin-top:16px;font-size:1em;font-style:italic;font-weight:bold}html body dl dd{padding:0 16px;margin-bottom:16px}html body code{font-family:Menlo,Monaco,Consolas,'Courier New',monospace;font-size:.85em !important;color:#000;background-color:#f0f0f0;border-radius:3px;padding:.2em 0}html body code::before,html body code::after{letter-spacing:-0.2em;content:"\00a0"}html body pre>code{padding:0;margin:0;font-size:.85em !important;word-break:normal;white-space:pre;background:transparent;border:0}html body .highlight{margin-bottom:16px}html body .highlight pre,html body pre{padding:1em;overflow:auto;font-size:.85em !important;line-height:1.45;border:#d6d6d6;border-radius:3px}html body .highlight pre{margin-bottom:0;word-break:normal}html body pre code,html body pre tt{display:inline;max-width:initial;padding:0;margin:0;overflow:initial;line-height:inherit;word-wrap:normal;background-color:transparent;border:0}html body pre code:before,html body pre tt:before,html body pre code:after,html body pre tt:after{content:normal}html body p,html body blockquote,html body ul,html body ol,html body dl,html body pre{margin-top:0;margin-bottom:16px}html body kbd{color:#000;border:1px solid #d6d6d6;border-bottom:2px solid #c7c7c7;padding:2px 4px;background-color:#f0f0f0;border-radius:3px}@media print{html body{background-color:#fff}html body h1,html body h2,html body h3,html body h4,html body h5,html body h6{color:#000;page-break-after:avoid}html body blockquote{color:#5c5c5c}html body pre{page-break-inside:avoid}html body table{display:table}html body img{display:block;max-width:100%;max-height:100%}html body pre,html body code{word-wrap:break-word;white-space:pre}}.markdown-preview{width:100%;height:100%;box-sizing:border-box}.markdown-preview .pagebreak,.markdown-preview .newpage{page-break-before:always}.markdown-preview pre.line-numbers{position:relative;padding-left:3.8em;counter-reset:linenumber}.markdown-preview pre.line-numbers>code{position:relative}.markdown-preview pre.line-numbers .line-numbers-rows{position:absolute;pointer-events:none;top:1em;font-size:100%;left:0;width:3em;letter-spacing:-1px;border-right:1px solid #999;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.markdown-preview pre.line-numbers .line-numbers-rows>span{pointer-events:none;display:block;counter-increment:linenumber}.markdown-preview pre.line-numbers .line-numbers-rows>span:before{content:counter(linenumber);color:#999;display:block;padding-right:.8em;text-align:right}.markdown-preview .mathjax-exps .MathJax_Display{text-align:center !important}.markdown-preview:not([for="preview"]) .code-chunk .btn-group{display:none}.markdown-preview:not([for="preview"]) .code-chunk .status{display:none}.markdown-preview:not([for="preview"]) .code-chunk .output-div{margin-bottom:16px}.scrollbar-style::-webkit-scrollbar{width:8px}.scrollbar-style::-webkit-scrollbar-track{border-radius:10px;background-color:transparent}.scrollbar-style::-webkit-scrollbar-thumb{border-radius:5px;background-color:rgba(150,150,150,0.66);border:4px solid rgba(150,150,150,0.66);background-clip:content-box}html body[for="html-export"]:not([data-presentation-mode]){position:relative;width:100%;height:100%;top:0;left:0;margin:0;padding:0;overflow:auto}html body[for="html-export"]:not([data-presentation-mode]) .markdown-preview{position:relative;top:0}@media screen and (min-width:914px){html body[for="html-export"]:not([data-presentation-mode]) .markdown-preview{padding:2em calc(50% - 457px + 2em)}}@media screen and (max-width:914px){html body[for="html-export"]:not([data-presentation-mode]) .markdown-preview{padding:2em}}@media screen and (max-width:450px){html body[for="html-export"]:not([data-presentation-mode]) .markdown-preview{font-size:14px !important;padding:1em}}@media print{html body[for="html-export"]:not([data-presentation-mode]) #sidebar-toc-btn{display:none}}html body[for="html-export"]:not([data-presentation-mode]) #sidebar-toc-btn{position:fixed;bottom:8px;left:8px;font-size:28px;cursor:pointer;color:inherit;z-index:99;width:32px;text-align:center;opacity:.4}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] #sidebar-toc-btn{opacity:1}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .md-sidebar-toc{position:fixed;top:0;left:0;width:300px;height:100%;padding:32px 0 48px 0;font-size:14px;box-shadow:0 0 4px rgba(150,150,150,0.33);box-sizing:border-box;overflow:auto;background-color:inherit}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .md-sidebar-toc::-webkit-scrollbar{width:8px}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .md-sidebar-toc::-webkit-scrollbar-track{border-radius:10px;background-color:transparent}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .md-sidebar-toc::-webkit-scrollbar-thumb{border-radius:5px;background-color:rgba(150,150,150,0.66);border:4px solid rgba(150,150,150,0.66);background-clip:content-box}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .md-sidebar-toc a{text-decoration:none}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .md-sidebar-toc ul{padding:0 1.6em;margin-top:.8em}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .md-sidebar-toc li{margin-bottom:.8em}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .md-sidebar-toc ul{list-style-type:none}html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .markdown-preview{left:300px;width:calc(100% -  300px);padding:2em calc(50% - 457px -  150px);margin:0;box-sizing:border-box}@media screen and (max-width:1274px){html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .markdown-preview{padding:2em}}@media screen and (max-width:450px){html body[for="html-export"]:not([data-presentation-mode])[html-show-sidebar-toc] .markdown-preview{width:100%}}html body[for="html-export"]:not([data-presentation-mode]):not([html-show-sidebar-toc]) .markdown-preview{left:50%;transform:translateX(-50%)}html body[for="html-export"]:not([data-presentation-mode]):not([html-show-sidebar-toc]) .md-sidebar-toc{display:none}
/* Please visit the URL below for more information: */
/*   https://shd101wyy.github.io/markdown-preview-enhanced/#/customize-css */

      </style>
    </head>
    <body for="html-export">
      <div class="mume markdown-preview  ">
      <h1 class="mume-header" id="saf%E9%A1%B9%E7%9B%AE%E7%BB%8F%E9%AA%8C%E5%88%86%E4%BA%AB-br-font-size4-university-of-california-berkeleyfont">SAF&#x9879;&#x76EE;&#x7ECF;&#x9A8C;&#x5206;&#x4EAB; <br> <font size="4"> <em>University of California - Berkeley</em></font></h1>

<hr>
<h2 class="mume-header" id="%E9%AD%8F%E5%98%89%E6%B6%A6-%E8%87%AA%E6%88%91%E4%BB%8B%E7%BB%8D">&#x9B4F;&#x5609;&#x6DA6; - &#x81EA;&#x6211;&#x4ECB;&#x7ECD;</h2>

<ul>
<li>&#x5927;&#x8FDE;&#x7406;&#x5DE5;&#x5927;&#x5B66;&#x5927;&#x56DB;&#x5B66;&#x751F;</li>
<li>2019&#x6625;&#x5B63;&#x53C2;&#x52A0;SAF&#x4F2F;&#x514B;&#x5229;&#x4EA4;&#x6362;&#x9879;&#x76EE;&#xFF0C;&#x79CB;&#x5B63;&#x5EF6;&#x671F;&#x4E00;&#x4E2A;&#x5B66;&#x671F;&#xFF0C;&#x5171;&#x4EA4;&#x6362;&#x4E00;&#x5E74;</li>
<li>&#x88AB;CMU(MSTV+Advanced Study)&#x3001;&#x54E5;&#x5927;&#x3001;&#x675C;&#x514B;&#x3001;UCSD&#x3001;USC&#x3001;&#x6CE2;&#x58EB;&#x987F;&#x5927;&#x5B66;&#x7B49;10&#x6240;&#x5927;&#x5B66;&#x5F55;&#x53D6;</li>
</ul>
<hr>
<h2 class="mume-header" id="%E7%9B%AE%E5%BD%95">&#x76EE;&#x5F55;</h2>

<ol>
<li>&#x8981;&#x4E0D;&#x8981;&#x51FA;&#x56FD;&#x4EA4;&#x6362;</li>
<li>&#x8981;&#x4E0D;&#x8981;&#x53BB;&#x4F2F;&#x514B;&#x5229;&#x4EA4;&#x6362;</li>
<li>&#x8981;&#x4E0D;&#x8981;&#x9009;&#x62E9;SAF&#x53BB;&#x4F2F;&#x514B;&#x5229;&#x4EA4;&#x6362;</li>
<li>&#x73B0;&#x5728;&#x80FD;&#x505A;&#x4EC0;&#x4E48;</li>
</ol>
<hr>
<h2 class="mume-header" id="1-%E8%A6%81%E4%B8%8D%E8%A6%81%E5%87%BA%E5%9B%BD%E4%BA%A4%E6%8D%A2">1 &#x8981;&#x4E0D;&#x8981;&#x51FA;&#x56FD;&#x4EA4;&#x6362;</h2>

<ul>
<li><strong>&#x82B1;10%&#x7684;&#x94B1;&#x4F53;&#x9A8C;&#x7F8E;&#x672C;</strong>
<ul>
<li>&#x666E;&#x901A;&#x7F8E;&#x672C;&#x4EF7;&#x683C;&#xFF1A;4&#x5E74;&#x8FD1;200&#x4E07;</li>
<li>&#x4EA4;&#x6362;&#x4EF7;&#x683C;&#xFF1A;&#x4E00;&#x5B66;&#x671F;&#x4E0D;&#x8DB3;20&#x4E07;</li>
<li>&#x4E00;&#x5B66;&#x671F;&#x8DB3;&#x591F;&#x4F53;&#x9A8C;&#x751F;&#x6D3B;&#x548C;&#x5B66;&#x4E60;&#x65B9;&#x6CD5;</li>
</ul>
</li>
<li><strong>&#x5FAE;&#x4FE1;&#x597D;&#x53CB;&#x6570;&#x91CF;&#x7FFB;&#x4E00;&#x500D;</strong> <!--拓宽人脉-->
<ul>
<li>&#x7ED3;&#x8BC6;&#x5168;&#x56FD;&#x5404;&#x5730;&#x7684;&#x5927;&#x5B66;&#x751F;</li>
</ul>
</li>
<li><strong>&#x4F53;&#x9A8C;&#x53E6;&#x4E00;&#x79CD;&#x8BFE;&#x7A0B;&#x4F53;&#x7CFB;</strong> <!--增强学习能力-->
<ul>
<li>&#x56FD;&#x5185;&#x662F;&#x82CF;&#x8054;&#x6559;&#x5B66;&#x4F53;&#x7CFB;&#xFF0C;&#x7F8E;&#x56FD;&#x7684;&#x6559;&#x80B2;&#x4F53;&#x7CFB;&#x5B8C;&#x5168;&#x4E0D;&#x540C;
<ul>
<li>&#x7B80;&#x5316;&#x6C42;&#x89E3;&#x903B;&#x8F91;&#xFF0C;&#x628A;&#x65F6;&#x95F4;&#x7559;&#x7ED9;&#x521B;&#x65B0;</li>
</ul>
</li>
</ul>
</li>
</ul>
<hr>
<h2 class="mume-header" id="2-%E8%A6%81%E4%B8%8D%E8%A6%81%E5%8E%BB%E4%BC%AF%E5%85%8B%E5%88%A9%E4%BA%A4%E6%8D%A2">2 &#x8981;&#x4E0D;&#x8981;&#x53BB;&#x4F2F;&#x514B;&#x5229;&#x4EA4;&#x6362;</h2>

<ul>
<li>&#x8BA9;&#x8BA1;&#x7B97;&#x673A;&#x52A9;&#x529B;&#x4F60;&#x7684;&#x4E13;&#x4E1A;&#x5B66;&#x4E60;</li>
<li>&#x6E05;&#x6670;&#x7684;&#x8BFE;&#x7A0B;&#x5B89;&#x6392;
<ul>
<li>&#x8BFE;&#x524D;Agenda</li>
<li>&#x8BFE;&#x540E;Discussion Session</li>
<li>&#x8BFE;&#x4E0B;bCourse</li>
</ul>
</li>
<li>&#x63A5;&#x8FD1;&#x6E7E;&#x533A;&#x516C;&#x53F8;&#x7684;&#x673A;&#x4F1A;
<ul>
<li>&#x8BFE;&#x4E0A;&#x8BA4;&#x8BC6;&#x7684;&#x540C;&#x5B66;&#x5E26;&#x6211;&#x53C2;&#x89C2;Uber&#x65E0;&#x4EBA;&#x9A7E;&#x9A76;&#x57FA;&#x5730;&#xFF0C;&#x5C06;&#x6765;&#x5B9E;&#x4E60;&#x5185;&#x63A8;</li>
</ul>
</li>
<li>&#x65C5;&#x6E38;
<ul>
<li>&#x4E00;&#x53F7;&#x516C;&#x8DEF;&#x81EA;&#x9A7E;</li>
<li>Yosemite Park&#x65E5;&#x51FA;</li>
<li>&#x516C;&#x4EA4;&#x8F66;&#x53EF;&#x8FBE;&#x6D77;&#x8FB9;</li>
</ul>
</li>
<li>&#x5B66;&#x4E60;&#x538B;&#x529B;</li>
<li>Extension workshop &amp; party</li>
</ul>
<hr>
<h2 class="mume-header" id="3-%E8%A6%81%E4%B8%8D%E8%A6%81%E9%80%89%E6%8B%A9saf%E5%8E%BB%E4%BC%AF%E5%85%8B%E5%88%A9%E4%BA%A4%E6%8D%A2">3 &#x8981;&#x4E0D;&#x8981;&#x9009;&#x62E9;SAF&#x53BB;&#x4F2F;&#x514B;&#x5229;&#x4EA4;&#x6362;</h2>

<ul>
<li>&#x73B0;&#x5B9E;&#x7248;&#x751F;&#x6D3B;&#x5927;&#x7206;&#x70B8;
<ul>
<li>12&#x4EBA;&#x7684;&#x5957;&#x95F4;&#xFF0C;&#x6BCF;&#x665A;&#x6B22;&#x4E50;&#x591A;&#x591A;</li>
<li>&#x6BCF;&#x5468;&#x53A8;&#x827A;&#x6BD4;&#x62FC;&#xFF0C;&#x6BCF;&#x665A;&#x9762;&#x70B9;&#x653E;&#x6BD2;</li>
</ul>
</li>
<li>&#x987A;&#x5229;&#x5B8C;&#x6210;&#x7B2C;&#x4E00;&#x6B21;&#x7559;&#x5B66;
<ul>
<li>&#x7701;&#x53BB;&#x7B7E;&#x8BC1;&#x56F0;&#x6270;&#xFF08;&#x6750;&#x6599;&#x51C6;&#x5907;&#x6307;&#x5BFC;&#xFF09;</li>
<li>&#x7701;&#x53BB;&#x79DF;&#x623F;&#x3001;lease&#x56F0;&#x6270;&#xFF08;&#x6C34;&#x5F88;&#x6DF1;&#xFF01;&#xFF09;</li>
<li>&#x5BF9;SF&#x673A;&#x573A;&#x4E0D;&#x719F;&#x6089;&#x7684;&#x8BDD;&#xFF0C;&#x52A0;&#x4E0A;&#x65F6;&#x5DEE;&#x52B3;&#x7D2F;&#xFF0C;&#x7B2C;&#x4E00;&#x6B21;&#x5F88;&#x96BE;&#x62B5;&#x8FBE;&#x6821;&#x56ED;</li>
</ul>
</li>
<li>&#x5FAE;&#x4FE1;&#x597D;&#x53CB;&#x6570;&#x91CF;&#x518D;&#x7FFB;&#x4E00;&#x500D;
<ul>
<li>SAF&#x7FA4;&#xFF0C;&#x805A;&#x96C6;&#x51E0;&#x4E4E;&#x6240;&#x6709;&#x4EA4;&#x6362;&#x751F;</li>
</ul>
</li>
<li>&#x751F;&#x6D3B;&#x79D8;&#x4E66;
<ul>
<li>&#x968F;&#x65F6;&#x6253;&#x7535;&#x8BDD;&#x7ED9;&#x7F8E;&#x56FD;&#x8D1F;&#x8D23;&#x4EBA;</li>
</ul>
</li>
</ul>
<hr>
<h2 class="mume-header" id="4-%E7%8E%B0%E5%9C%A8%E8%83%BD%E5%81%9A%E4%BB%80%E4%B9%88">4 &#x73B0;&#x5728;&#x80FD;&#x505A;&#x4EC0;&#x4E48;</h2>

<ul>
<li>&#x6A21;&#x62DF;&#x7533;&#x8BF7;
<ul>
<li>&#x63D0;&#x524D;&#x4E86;&#x89E3;&#x7406;&#x60F3;&#x5B66;&#x6821;&#x5BF9;&#x4EA4;&#x6362;&#x7ECF;&#x5386;&#x7684;&#x770B;&#x91CD;&#x7A0B;&#x5EA6;</li>
</ul>
</li>
<li>&#x4E86;&#x89E3;&#x6559;&#x6388;
<ul>
<li>&#x5230;&#x6559;&#x6388;&#x4E2A;&#x4EBA;&#x4E3B;&#x9875;&#x4E0A;&#x770B;&#x8BBA;&#x6587;&#xFF0C;&#x63D0;&#x524D;&#x4E86;&#x89E3;&#x5176;&#x7814;&#x7A76;&#x65B9;&#x5411;</li>
</ul>
</li>
<li>&#x8BED;&#x8A00;&#x6210;&#x7EE9;
<ul>
<li>&#x53C2;&#x52A0;&#x9879;&#x76EE;&#x7684;&#x552F;&#x4E00;&#x786C;&#x6027;&#x8981;&#x6C42;</li>
</ul>
</li>
</ul>

      </div>
      
      
    
    
    
    
    
    
    
    
  
    </body></html>
