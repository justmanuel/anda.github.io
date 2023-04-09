---
title: "Gh Issues"
date: 2023-04-09T16:30:44-04:00
draft: false
---

Hello, this page is to track issues I had along the way with deploying my website using GoHugo with cloudflare and github/pages.

I am currently using Visual Studio Code along for Windows OS. So you can understand my frustration when I also have to use fake Git Bash.

Currently the first main issue I faced was a BIG Error on my website when trying to run it locally:

``` page not found ```

I got a few warnings:

``` found no layout file for "HTML" for kind "page": You should create a template file which matches Hugo Layouts Lookup Rules for this combination. ```

However, the template and website were both working properly and could be seen in my GitHub repo. I luckily turned to good ole Google and found a comment stating that it would be from submodules not being cloned along with the repo.

I used:

``` git clone --recurse-submodules https://github.com/example/example {insert your github repo instead} ```

This seemed to work and I could again test my hugo website locally before pushing to my repo and making the change live. 
