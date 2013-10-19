---
layout: post
title: "Git Ignore file permissions"
date: 2013-07-29 16:01
comments: true
categories: code, git
---

If you use git a lot (like me) and very often have to share git repo/directory between machines. Here is how you can make git not to consider file-permission changes as modifications (shown in your `git status`).

- Got to repo and execute:
```
git config core.filemode false
```

- To make it permanent & add to your global config:
```
git config --global core.filemode false
```

