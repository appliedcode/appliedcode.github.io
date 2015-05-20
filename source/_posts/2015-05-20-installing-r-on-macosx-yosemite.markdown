---
layout: post
title: "Installing R on MacOSX Yosemite"
date: 2015-05-20 18:45
comments: true
categories: R, HomeBrew
---

Here is how you can install [Programming Language R](http://en.wikipedia.org/wiki/R_%28programming_language%29) on MacOSX Yosemite

Step 1: You need [HomeBrew](http://brew.sh/), its pretty easy, please visit http://brew.sh/ for instruction to install [HomeBrew](http://brew.sh/).

Step 2: Open Terminal, execute the following,
          brew tap homebrew/science
          brew install gcc
          brew install r

The gcc package is the homebrew/science tap already contains the latest fortran compiler(gfortran), and most of all: the whole package is precompiled so it saves you a lot of compilation time.

[Mohit](https://twitter.com/mohitsethi)