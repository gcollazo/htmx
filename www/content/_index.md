+++
insert_anchor_links = "left"
+++

<div class="dark-hero full-width" classes="add appear">
  <span class="logo dark">&lt;<a>/</a>&gt; <span class="no-mobile">htm<a>x</a></span></span>
  <sub class="no-mobile"><i>high power tools for HTML</i></sub>
</div>


<h2>introduction</h2>

htmx gives you access to [AJAX](@/docs.md#ajax), [CSS Transitions](@/docs.md#css_transitions), [WebSockets](@/docs.md#websockets) and [Server Sent Events](@/docs.md#sse) 
directly in HTML, using [attributes](@/reference.md#attributes), so you can build 
[modern user interfaces](@/examples/_index.md) with the [simplicity](https://en.wikipedia.org/wiki/HATEOAS) and 
[power](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm) of hypertext

htmx is small ([~14k min.gz'd](https://unpkg.com/htmx.org/dist/)), 
[dependency-free](https://github.com/bigskysoftware/htmx/blob/master/package.json),
[extendable](@/extensions/_index.md), 
IE11 compatible & has **reduced** code base sizes by [67% when compared with react](@/essays/a-real-world-react-to-htmx-port.md)

<h2>motivation</h2>

* Why should only [`<a>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) and [`<form>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form) be able to make HTTP requests?
* Why should only [`click`](https://developer.mozilla.org/en-US/docs/Web/API/Element/click_event) & [`submit`](https://developer.mozilla.org/en-US/docs/Web/API/HTMLFormElement/submit_event) events trigger them?
* Why should only [`GET`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/GET) & [`POST`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/POST) methods be [available](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)?
* Why should you only be able to replace the **entire** screen?

By removing these arbitrary constraints, htmx completes HTML as a [hypertext](https://en.wikipedia.org/wiki/Hypertext)

<h2>quick start</h2>

```html
  <script src="https://unpkg.com/htmx.org@1.9.0"></script>
  <!-- have a button POST a click via AJAX -->
  <button hx-post="/clicked" hx-swap="outerHTML">
    Click Me
  </button>
```

The [`hx-post`](@/attributes/hx-post.md) and [`hx-swap`](@/attributes/hx-swap.md) attributes on
this button tell htmx:

> "When a user clicks on this button, issue an AJAX request to /clicked, and replace the entire button with the HTML response"

htmx is the successor to [intercooler.js](http://intercoolerjs.org)

Read the [docs introduction](@/docs.md#introduction) for a more in-depth... introduction.

<h2>sponsors</h2>

A huge thank you to all our <a href="https://github.com/sponsors/bigskysoftware?o=esb">sponsors</a>, including:

<div class="row" style="text-align: center">
<div class="col 2" style="padding: 16px">
<a href="https://www.jetbrains.com//"><img src="/img/jetbrains.png" style="max-width:30%;min-width:200px;"></a>
</div>
</div>
<div class="row" style="text-align: center">
<div class="col 2" style="padding: 16px">

<a href="https://www.commspace.co.za/"><img class="shift-up-img" src="/img/commspace.svg" style="width:100%;max-width:200px"></a>

</div>

<div class="col 2" style="padding: 0">
</div>

<div class="col 2" style="padding: 16px">

<a href="https://craftcms.com"><img class="shift-up-img" src="/img/logo-craft-cms.svg" style="width:90%;max-width:200px"></a>

</div>
</div><div class="row" style="text-align: center">
<div class="col 2" style="padding: 16px">
<a href="https://buttercms.com/?utm_campaign=sponsorship&utm_medium=banner&utm_source=htmxhome"><img class="shift-up-img" src="/img/butter-cms.svg" style="width:100%;max-width:200px"></a>
</div>

<div class="col 2" style="padding: 0;">
</div>

<div class="col 2" style="padding: 16px">
<a href="https://bigsky.software"><img class="shift-up-img" src="/img/bss.png" style="width:100%;max-width:200px"></a>

</div>
</div>

<div style="text-align: center;font-style: italic;margin-top: 26px;">ʕ •ᴥ•ʔ made in montana</div>
