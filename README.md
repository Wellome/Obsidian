README            body{--line-width:40em;--line-width-adaptive:40em;--file-line-width:40em;--sidebar-width:min(20em, 80vw);--collapse-arrow-size:11px;--tree-horizontal-spacing:0.6em;--tree-vertical-spacing:0.6em;--sidebar-margin:12px}.sidebar{height:100%;min-width:calc(var(--sidebar-width) + var(--divider-width-hover));max-width:calc(var(--sidebar-width) + var(--divider-width-hover));font-size:14px;z-index:10;position:relative;overflow:hidden;transition:min-width ease-in-out,max-width ease-in-out;transition-duration:.2s;contain:size}.sidebar-left{left:0}.sidebar-right{right:0}.sidebar.is-collapsed{min-width:0;max-width:0}body.floating-sidebars .sidebar{position:absolute}.sidebar-content{height:100%;min-width:calc(var(--sidebar-width) - var(--divider-width-hover));top:0;padding:var(--sidebar-margin);padding-top:4em;line-height:var(--line-height-tight);background-color:var(--background-secondary);transition:background-color,border-right,border-left,box-shadow;transition-duration:var(--color-fade-speed);transition-timing-function:ease-in-out;position:absolute;display:flex;flex-direction:column}.sidebar:not(.is-collapsed) .sidebar-content{min-width:calc(max(100%,var(--sidebar-width)) - 3px);max-width:calc(max(100%,var(--sidebar-width)) - 3px)}.sidebar-left .sidebar-content{left:0;border-top-right-radius:var(--radius-l);border-bottom-right-radius:var(--radius-l)}.sidebar-right .sidebar-content{right:0;border-top-left-radius:var(--radius-l);border-bottom-left-radius:var(--radius-l)}.sidebar:has(.sidebar-content:empty):has(.topbar-content:empty){display:none}.sidebar-topbar{height:2em;width:var(--sidebar-width);top:var(--sidebar-margin);padding-inline:var(--sidebar-margin);z-index:1;position:fixed;display:flex;align-items:center;transition:width ease-in-out;transition-duration:inherit}.sidebar.is-collapsed .sidebar-topbar{width:calc(2.3em + var(--sidebar-margin) \* 2)}.sidebar .sidebar-topbar.is-collapsed{width:0}.sidebar-left .sidebar-topbar{left:0}.sidebar-right .sidebar-topbar{right:0}.topbar-content{overflow:hidden;overflow:clip;width:100%;height:100%;display:flex;align-items:center;transition:inherit}.sidebar.is-collapsed .topbar-content{width:0;transition:inherit}.clickable-icon.sidebar-collapse-icon{background-color:transparent;color:var(--icon-color-focused);padding:0!important;margin:0!important;height:100%!important;width:2.3em!important;margin-inline:0.14em!important;position:absolute}.sidebar-left .clickable-icon.sidebar-collapse-icon{transform:rotateY(180deg);right:var(--sidebar-margin)}.sidebar-right .clickable-icon.sidebar-collapse-icon{transform:rotateY(180deg);left:var(--sidebar-margin)}.clickable-icon.sidebar-collapse-icon svg.svg-icon{width:100%;height:100%}.sidebar-section-header{margin:0 0 1em 0;text-transform:uppercase;letter-spacing:.06em;font-weight:600}body{transition:background-color var(--color-fade-speed) ease-in-out}.webpage-container{display:flex;flex-direction:row;height:100%;width:100%;align-items:stretch;justify-content:center}.document-container{opacity:1;flex-basis:100%;max-width:100%;width:100%;height:100%;display:flex;flex-direction:column;align-items:center;transition:opacity .2s ease-in-out;contain:inline-size}.hide{opacity:0;transition:opacity .2s ease-in-out}.document-container>.markdown-preview-view{margin:var(--sidebar-margin);margin-bottom:0;width:100%;width:-webkit-fill-available;width:-moz-available;width:fill-available;background-color:var(--background-primary);transition:background-color var(--color-fade-speed) ease-in-out;border-top-right-radius:var(--window-radius,var(--radius-m));border-top-left-radius:var(--window-radius,var(--radius-m));overflow-x:hidden!important;overflow-y:auto!important;display:flex!important;flex-direction:column!important;align-items:center!important;contain:inline-size}.document-container>.markdown-preview-view>.markdown-preview-sizer{padding-bottom:80vh!important;width:100%!important;max-width:var(--line-width)!important;flex-basis:var(--line-width)!important;transition:background-color var(--color-fade-speed) ease-in-out;contain:inline-size}.markdown-rendered img:not(\[width\]),.view-content img:not(\[width\]){max-width:100%;outline:0}.document-container>.view-content.embed{display:flex;padding:1em;height:100%;width:100%;align-items:center;justify-content:center}.document-container>.view-content.embed>\*{max-width:100%;max-height:100%;object-fit:contain}:has(> :is(.math,table)){overflow-x:auto!important}.document-container>.view-content{overflow-x:auto;contain:content;padding:0;margin:0;height:100%}.scroll-highlight{position:absolute;width:100%;height:100%;pointer-events:none;z-index:1000;background-color:hsla(var(--color-accent-hsl),.25);opacity:0;padding:1em;inset:50%;translate:-50% -50%;border-radius:var(--radius-s)}async function loadIncludes(){if("file:"!=location.protocol){let e=document.querySelectorAll("include");for(let t=0;t<e.length;t++){let o=e\[t\],l=o.getAttribute("src");try{const e=await fetch(l);if(!e.ok){console.log("Could not include file: "+l),o?.remove();continue}let t=await e.text(),n=document.createRange().createContextualFragment(t),i=Array.from(n.children);for(let e of i)e.classList.add("hide"),e.style.transition="opacity 0.5s ease-in-out",setTimeout((()=>{e.classList.remove("hide")}),10);o.before(n),o.remove(),console.log("Included file: "+l)}catch(e){o?.remove(),console.log("Could not include file: "+l,e);continue}}}else{if(document.querySelectorAll("include").length>0){var e=document.createElement("div");e.id="error",e.textContent="Web server exports must be hosted on an http / web server to be viewed correctly.",e.style.position="fixed",e.style.top="50%",e.style.left="50%",e.style.transform="translate(-50%, -50%)",e.style.fontSize="1.5em",e.style.fontWeight="bold",e.style.textAlign="center",document.body.appendChild(e),document.querySelector(".document-container")?.classList.remove("hide")}}}document.addEventListener("DOMContentLoaded",(()=>{loadIncludes()}));let isFileProtocol="file:"==location.protocol;function waitLoadScripts(e,t){let o=e.map((e=>document.getElementById(e+"-script"))),l=0;!function e(){let n=o\[l\];l++,n&&"true"!=n.getAttribute("loaded")||l<o.length&&e(),l<o.length?n.addEventListener("load",e):t()}()}

let theme=localStorage.getItem("theme")||(window.matchMedia("(prefers-color-scheme: dark)").matches?"dark":"light");"dark"==theme?(document.body.classList.add("theme-dark"),document.body.classList.remove("theme-light")):(document.body.classList.add("theme-light"),document.body.classList.remove("theme-dark")),window.innerWidth<480?document.body.classList.add("is-phone"):window.innerWidth<768?document.body.classList.add("is-tablet"):window.innerWidth<1024?document.body.classList.add("is-small-screen"):document.body.classList.add("is-large-screen")

let ls = document.querySelector(".sidebar-left"); ls.classList.add("is-collapsed"); if (window.innerWidth > 768) ls.classList.remove("is-collapsed"); ls.style.setProperty("--sidebar-width", localStorage.getItem("sidebar-left-width"));

    tags:
      - INDEX

Obsidian


============

A website version of my brain. Updated whenever I feel like it.

Welcome!
----------

Hello, whoever is reading this. I hope you enjoy the website, or the raw code if you're into that stuff (wouldn't blame you). I've ommitted all my Daily notes from here, as to protect the privacy of both me and my friends. Respectfully, do not take any code you find in here. If you do, I'll... give you a very stern rant.

Why?
------

Why what? Why upload all of my notes detailing my school work, assignments, etc? I can. Plus, it's a backup. If, for some godforsaken reason, someone steals my laptop, PC, 2tib harddrive, all of my USBs, deletes my Google Account and my phone(s), well, I'm not able to access my notes, but at least I have a backup (good luck stealing all of that, though, I hide stuff pretty well if I say so myself). If they delete my GitHub account on top of all of this, I am screwed (unless I've given a copy of this to others).

Who is this for?
------------------

Me, myself, and anyone else. It's my thoughts, my life, hell, you can even just say it's who I am. The projects I work on, the notes I take, every word I type, it all links back to who I am. By reading this, I hope you get a better understanding of who I am, because, honestly, I barely have an understanding of who I am in this world.

Final Notes
===========

As I stated before, I've ridded this vault of all mentions of my friends names (as to protect their privacy), and removed my Daily Notes, to protect mine. I hope you enjoy wandering through this ever-growing garden of my thoughts (I'm not done with porting all my notes over, give it a week, and it should be like triple the size).

Here's a starting point.
--------------------------

[00 - MAIN PAGE](00-index/00-main-page.html)

Interactive Graph

Table Of Contents

[

Obsidian

](readme.html#Obsidian)

[

Welcome!

](readme.html#Welcome!)

[

Why?

](readme.html#Why?)

[

Who is this for?

](readme.html#Who_is_this_for?)

[

Final Notes

](readme.html#Final_Notes)

[

Here's a starting point.

](readme.html#Here's_a_starting_point.)

let rs = document.querySelector(".sidebar-right"); rs.classList.add("is-collapsed"); if (window.innerWidth > 768) rs.classList.remove("is-collapsed"); rs.style.setProperty("--sidebar-width", localStorage.getItem("sidebar-right-width"));
