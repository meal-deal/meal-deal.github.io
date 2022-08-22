---
title: "Simpler Front-end Toolset"
date: 2020-08-11T11:47:12+04:00
slug: 2020-08-11-simple-front-end
type: posts
tags:
  - web
---

When looking to start a simple front end project, many people may default to using things like React, TypeScript, Vite, or Tailwind.

Instead, here are some recommendations that <mark>don't require using Node or NPM.</mark>

## CSS
Use a "classless" CSS library like [CSSBed](https://www.cssbed.com/) or [Pico.css](https://picocss.com/)</a>. 

It's similar to Bootstrap, but doesn't require writing any CSS or adding any CSS classes to your HTML. Just include the &lt;link&gt; tag in your HTML document.

If you prefer to try a utility based approach, similar to the "Tailwind" everyone keeps raving about, try [Basscss](https://basscss.com/). Again, no tooling, just need a <link> tag.

## JavaScript
For adding some interactivity to your site, [htmx](https://htmx.org/) is a pretty simple approach. If you really want something like React, then [Mithril.js](https://mithril.js.org/) is quite similar but much simpler.
