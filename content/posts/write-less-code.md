---
title: "Write Less Code"
date: 2022-06-16T22:28:53+04:00
tags:
  - engineering
---


We enjoy writing code, solving problems. It’s exciting to build something new.

We seek out new languages, paradigms, frameworks, stacks, tools, APIs, and libraries to learn. Immersing ourselves in them and seeking mental flow – that state in which we generate new code as hours feel like minutes.

Some misguided people have gone so far as to use lines of code generated per hour as a metric of productivity.  But even if you we don't get all the way to the point of weapons-grade stupidity, it’s still easy to believe that more code = better.  

Code is the DNA of your app and your business, and so naturally companies consider it valuable intellectual property.

Forget all that. It's nonsense.

The reality is that code is a complete and total liability.

## Less Is Usually More

You know what’s better than doing in 5 lines of code what someone else did in 100?  Doing it with 0 lines of code.

Go ahead, let's write a simply line of code:

```php
echo(“Hello World!”);
```

How many things could go wrong with this simple and common line?

- Would this code actually run in an environment that allows printing?
- Would that magic string end up being a problem later?
- Shouldn’t you be using logging instead? Isn't that the best practice?
- Did you think about the security implications of this code?

Let's conservatively say that there are 10 things that could go wrong with this one line of code.  So then, we add another line of code.

You might then assume that this brings the total to 20 things that could go wrong?

I would argue that it more closer to 100. Maybe I'm a pessimist, but I really think that the relationship between potential issues and lines of code is closer to a combinatoric one than a linear one.

Do you know what generally correlates more than anything else with undesirable codebase properties?  The size of the codebase.

Pretty much everything bad about a codebase has a strong relationship with the size of the codebase, measured in lines of code.

I think you should always strive to do everything using as little code as humanly possible.