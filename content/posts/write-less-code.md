---
title: "Write Less Code"
date: 2022-06-16T22:28:53+04:00
tags:
  - engineering
---


It feels good to write code, to solve problems, and it’s exciting to build something new.

Developers often seek out new languages, new paradigms, frameworks, stacks, tools, APIs, and libraries to learn. We immerse ourselves in them and seek mental flow – that state in which we happily generate new code.

Some misguided genuises have even gone so far as to take lines of code generated per hour as a metric of overall productivity.  But even if you we don't get all the way to the point of weapons-grade stupidity, it’s still easy to think that somehow more code is better.  Code is essentially the DNA of your killer app and your business, and so naturally companies consider it valuable intellectual property.

Now, forget all that. It's nonsense.

I can totally understand why we do look at code as an asset.  However, the reality is that code is a complete and total liability.

## Less Is Usually More

You know what’s actually better than doing in 5 lines of code what someone else did in 100?  Doing it with 0 lines of code.

Go ahead, let's write a simply line of code:

echo(“Hello World!”);

How many things do you think could go wrong in this scenario?

- Would this code actually run in an environment that allows console printing?
- Would that magic string end up being a problem later?
- Shouldn’t you be logging instead? Isn't that the best practice?
- Did you even think about the security implications of this code?

Now, let us conservatively say that there are 10 things that could go wrong with this line of code.  So then, we add another line of code.

Would you then assume that this then brings the total to 20 things that could go wrong?

I would argue that it more likely brings it closer to 100. You can call me a pessimist, but I really think that the relationship between potential issues and lines of code is closer to combinatoric one than a linear one.

Do you know what generally correlates more than anything else with undesirable codebase properties?  The size of the codebase.

Pretty much everything bad about a codebase has a significant relationship with the actual size of the codebase, measured in lines of code.

I also love writing code, I enjoy studying it, analyzing it, and building things.  But make no mistake, it’s a huge liability.  

You should always strive to do everything using as little code as humanly possible.