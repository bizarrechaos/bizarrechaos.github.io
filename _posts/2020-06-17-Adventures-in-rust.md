---
layout: post
title: "Adventures in rust"
date:	2020-17-17 19:54
categories:
    - posts
tags:
    - cli
    - tools
    - rust
---

It has been awhile since my last post.
I need to jump back into the RE excercises and get some of that documented, however lately I have been diving into rust.

Most of my programming/coding previously has been in python.
Don't get wrong, I love and still use and write python daily, however I wanted something different.

Recently I've been playing with rust.
Rust is a compiled language that is built for security and speed.
While none of the concepts I know and love really translate to rust I thought it was something I wanted to take on.
I have been following the official [The Rust Programming Language Book](https://doc.rust-lang.org/stable/book/)

So far it has been a great expierence and I look forward to developing some new tools.
My first project is something I have wanted for awhile (and there are likely alternative already out there).
I wrote a script in python a few years ago to take a filepath and print multiple hashes for that file.
It worked without issue, the problem was the speed at which it ran.
This wasn't an issue unless you wanted to has several files all at once, a common task for the budding malware analyst.
So doing some research I looked into rust and discovered I could do what I wanted in rust, and I could do it fast.

Introducing [hashy](https://github.com/bizarrechaos/hashy)

<script id="asciicast-Ov8vSYAtuvBdJGvmE1lnmBMWd" src="https://asciinema.org/a/Ov8vSYAtuvBdJGvmE1lnmBMWd" async></script>

Feel free to check it out and contribute if you feel inclined.
I have absolutely no idea what I am doing in rust so I expect this can be made exceptionally better.