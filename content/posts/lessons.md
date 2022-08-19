---
title: "A Few Things I've Learnt"
date: 2022-08-16T10:55:09+04:00
tags:
  - engineering
---

Every couple of years the people you work with changes. New developers don’t understand the problems of the past because they've never seen them. Older developers burn out or lose excitement. New developers have a different reference frame, and they learn in different ways. 

When you fix an issue, you should really understand the issue that you’re fixing. Take a few step back and try to re-integrate any new knowledge into the design. Should anything change? Sometimes, solving the wrong problem can spawn 10 new problems.

Long-running branches are a hassle to maintain. Always merge regularly and keep your code behind a feature flag. Put time into having a good feature flag mechanism that cuts out any bad code and/or lets you deploy feature flag changes for a certain percentage of users in production.

If you fix a bug, you should also add a test that fails. If you don’t add, you’re implicitly accepting that someone else (even you) will break it again in the future.

Some projects you work on, will have a wide surface area and decisions need to be decentralised. Other times, the projects will have a narrow surface area and decisions need to be centralised. Both styles are good,  but don’t get confused as to why techniques that work for one type of project may be impractical or disastrous for another