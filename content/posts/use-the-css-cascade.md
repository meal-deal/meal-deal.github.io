---
title: "Leveraging the CSS Cascade"
date: 2021-05-14T13:39:40+04:00
tags:
  - engineering
  - css
---

The CSS cascade can be your friend, if you learn to think about your CSS as layers:

- Have a settings stylesheet that contains all of your default variables.
- Followed by a base stylesheet that acts as a foundation.
- Then your layout stylesheets. Each one should be a self-contained layout or composition without depending on other stylesheets.
- Finally, your Block stylesheets that are the patterns to your composition, these are the recurring themes of your design. And the utilities that do one thing and one thing only.
  
You should the load your styles in that order. 

Your utilities should override your patterns, your patterns should override your compositions, your compositions should override your element styles, and the variables from everything else should override your default variables. 