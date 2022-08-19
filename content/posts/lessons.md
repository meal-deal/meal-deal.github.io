---
title: "Five More Lessons"
date: 2021-06-16T10:55:09+04:00
tags:
  - engineering
---

1. Every couple of years the industry changes, and so do the people you work with. New developers don’t understand the problems of the past because they've never seen them. Older developers burn out or lose excitement. New developers have a different reference frame, and they learn in different ways. 


2. When you fix an issue, you should really understand the issue that you’re fixing. Take a few steps back and try to re-integrate any new knowledge into the design. Should anything change? Sometimes solving the wrong problem can create a dozen new problems.


3. Long-running branches are a hassle. Always merge regularly and keep your code behind a feature flag. Put time into having a good feature flag mechanism that cuts out any bad code and/or lets you deploy feature flag changes for a certain percentage of users in production. 

4. If you fix a bug, you should also add a test that fails. If you don’t, you’re implicitly accepting that someone (even you) will break it again in the future.

5. Some projects have a wide surface area and decisions need to be decentralised. Other projects will have a narrow surface area and decisions need to be centralised. Both styles are ok,  but don’t get confused as to why techniques that work for one type of project may be impractical or disastrous for another