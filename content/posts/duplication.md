---
title: "Don't Repeat Yourself"
date: 2022-05-14T13:29:27+04:00
tags:
  - engineering
---


If someone hasn’t yet lectured you about copying code in your application, pasting it, then adjusting it (the “copy, paste, and adjust to taste” anti-pattern), consider this your lecture.

Let's imagine you have a perfectly good CalculateTax() method, but the product manager comes along and asks, “we’re onboarding new customers in Germany, and they calculate taxes a little differently there.”  So you then copy the current method, paste it, rename it CalculateTaxGermany() and tweak it as needed.

Here are some problems with this approach:

1. If a future update requires changes to the core logic, you now have to do the extra work and modify 2 methods. 
2. You now have created two chances to introduce bugs during these changes.
3. You’ve established a bad ‘design pattern’ and your code is ready for more redundant methods as your anti-pattern expansion continues.
4. Your work is going to increase exponentially as you go.
5. It’s then only a matter of time before you introduce more bugs by forgetting to change things everywhere you now need to.
6. Eventually, all of these methods will differ from each other just enough that you can no longer easily merge them back together and fix the whole mess, but they also won't differ so much that you can avoid making 20 changes every time someone updates a taxation rule.

It’s really a horrible mess.  This copy-paste anti-pattern is only the surface level problem.

The real underlying problem is the general duplication of knowledge in your codebases.

Duplication of knowledge in your code can occur in many ways, lazy copy-pasta is just the most obvious version.  

Here are some more insiduous examples of duplicate knowledge:

- A for loop and with a comment above it explaining the start, end, and increment values.
  
- A global variable given a value inline and then re-assigned another value from a configuration file.

- A database table with columns “taxTotal,” “Tax,” and “Total”

In the case of a unnecessary code comment, it could just be the team’s chief nagging officer brow-beating you into always checking or adding comments when you update code.

You should always ruthlessly resist duplication of knowledge anywhere in your codebases.