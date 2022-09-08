---
title: "Don't Repeat Yourself"
date: 2022-05-14T13:29:27+04:00
tags:
  - engineering
---


Imagine you have a  CalculateTax() method, but the product manager comes along and asks, “we’re expanding to Germany, and they calculate taxes a little differently there.”  So you then copy the current method, paste it, rename it CalculateTaxGermany() and tweak it as needed.

Here are some problems with this approach:

1. If a future update requires changes to the core logic, you now have to do the extra work and modify 2 methods. 
2. You now have created two chances to introduce bugs during these changes.
3. Your work is going to increase exponentially as you go.
4. It’s then only a matter of time before you introduce more bugs by forgetting to change things everywhere you now need to.
5. Eventually, all of these methods will differ from each other just enough that you can no longer easily merge them back together and fix the whole mess, but they also won't differ so much that you can avoid making 20 changes every time someone updates a taxation rule.

It’s quickly becomes hard to manage,  and this anti-pattern is only the surface level problem.

The real problem is the general duplication of knowledge in your codebases. 

Here are some more examples of duplicate knowledge:
- A for loop and with a comment above it explaining the start, end, and increment values.
- A global variable given a value inline and then re-assigned another value from a configuration file.
- A database table with columns “taxTotal,” “Tax,” and “Total”

You should always ruthlessly resist duplication of knowledge anywhere in your codebases.