---
layout: post
title: "Xcode Command Line Tools"
date: 2012-02-17 11:26
comments: true
categories:
---

Link to GCC package guy's post

Uninstall Xcode

- remove /Developer
- two commands to uninstall

sudo /Developer-3.2.6/Library/uninstall-devtools
sudo /Developer/Library/uninstall-devtools --mode=all /thx

Download the code tools and install

Homebrew issue link and fix

sudo ln -sf /usr/bin/llvm-gcc-4.2 /usr/bin/gcc-4.2
