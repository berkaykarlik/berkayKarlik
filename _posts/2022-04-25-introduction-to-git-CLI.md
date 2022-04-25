---
layout: post
title:  "Introduction to Version Control"
date:   2022-04-25 21:06:00 +0300
---

**Aimed Audiance Level: Never heard of version control of before**

## What is version control?
Whether it's your job or your hobby projects if you are programming more than a hello-world application, you surely need to use a version controlling tool. A version controlling tool allows you to track the progression of your code-base, to work on different features concurrently, to see historic versions and to work on the same code-base concurrently with your team.

## Why to use version control?
* I assume you have probably come across to bugs in your programs at this point. Have you ever lost your last steps and failed to go back to last working version? If not just continue programming without version control a little bit more and I promise it will happen.
* Many of newbie programmers use the most primitive version controlling, which is copying your projects entire folder and renaming it. However as your codebases grow, this becomes unsustainable. Are you going to check 100 different version to see the point of history where a single line added to codebase?
* Without version control it's very hard for multiple people to cooperate for large-scale projects. Imagine you are working with 20-100 people and they all have their own version of the project or even just part of the projects. Everybody would have to keep track of the files they have changed.
* Even if you think you can make your project in modular-decoupled (independent) pieces, at some point all these modules will have to be combined together. And then bug fixes & maintanence will be added on top of them. Without ability to backtrack your and your colleagues steps, you will spend most of your time debugging.
* Using version control tool that has a remote storage (GitHub for example) allows you to switch between devices without spending extra effort to transport your code. You can send/receive your latest version via version control tool as long as you have an internet connection.

## How to start version control?
Git is the most popular version control tool and almost all software companies expect you to use it. So I suggest you start from there. Also, Git is the name of the version control software and shouldn't be considered same with GitHub. GitHub is the storage platform that git can use (optinal and has alternatives) as a remote storage.

## Suggested Resources
* https://github.com/git-guides
* https://git-scm.com/book/en/v2
* https://learngitbranching.js.org/
* https://eagain.net/articles/git-for-computer-scientists/ (advanced)
