---
title: "Accessible Copy"
date: 2022-02-22T13:44:19+04:00
tags:
  - accessibility
  - html
---

- When writing, it's important to use plain language and avoid figures of speech, idioms, and complicated metaphors. You can use this [readability analyser](https://datayze.com/readability-analyzer.php) to asssess how accessible your copy is.

- The text content of `button`, `a`, and `label` elements should be unique and descriptive. You can also use visually hidden elements to add more context to these elements if your visual copy needs to be short.

- Center-aligned or justified text is difficult to read. Always prefer left-aligned text for left-to-right (LTR) languages, and right-aligned text for right-to-left (RTL) languages.

- Make sure the viewport zoom is not disabled. Many people will need to increase text-sizes to a point where they can read it. You should not stop them from doing this, even for web apps which favour a native app-like experience. Native apps should always respect Operating System settings for text resizing.

- Make sure your `title` is unique for every page. The title element, found in the document's head element, is usually the first bit of information announced by assistive technology. This then helps people to understand what page or view they are going to start navigating.

- Ensure your content flows linearly. Always remove any `tabindex` attribute values that are not either `0` or `-1`. Those elements that are natively focusable, like `links` or `button` elements, do not require a `tabindex`. Those elements which are not natively focusable should not have a `tabindex` applied to them except for very specific use cases.

- Make sure to have only one `h1` element per page. The `h1` element is used to communicate the higher-level purpose of the page. So, be careful not use the `h1` element for a heading that does not change between pages (like the site's name).