---
title: "Accessible Copy"
date: 2022-02-22T13:44:19+04:00
tags:
  - accessibility
  - html
---

- When writing, it's important to use plain language and avoid figures of speech, idioms, and complicated metaphors. 

- The text content of `button`, `a`, and `label` elements should be unique and descriptive. You can also use visually hidden elements to add more context to these elements if your visual copy needs to be short.

- Make sure your `title` is unique for every page. This helps people to understand what page or view they are going to start navigating.

- Ensure your content flows linearly. Remove any `tabindex` attribute values that are not either `0` or `-1`. Those elements that are natively focusable, like `links` or `button` elements, do not require a `tabindex`. Those elements which are not natively focusable should not have a `tabindex` applied to them except for very specific use cases.

- Use only one `h1` element per page. The `h1` element is used to communicate the higher-level purpose of the page. So, be careful not use the `h1` element for a heading that does not change between pages (like the site's name).