---
layout: post
title: "Adventures in Assembly"
date:	2019-07-06 22:00
categories:
    - posts
tags:
    - re
    - asm
---

For the past month I have been on a journey, an adventure even, to learn assembly code (x86 specifically).
The end result is to be able to read assembly code and move into more in depth malware analysis.

I found an online course that I think is great so far:
['xorpd - Assembly Language Adventures: Complete'](https://www.udemy.com/x86-asm-foundations/?couponCode=xorpd_website_20)

The author and instructor xorpd has a great site as well:
['xorpd.net'](https://www.xorpd.net/)

On his site you can find some great references for Assembly Language.
The course will take you from 0 knowledge about computers to a very good foundation in x86 Assembly.
He does stick with Windows and FASM in his course, but most of the excercises have been translated to YASM and will run on linux.

I also came across a neat little go program that helps to emulate x86 or x64 systems and gives you visual representation of the registers and stack as you enter instructions.
It is kind of like an assembly language interpreter or cli.
['asm-cli'](https://github.com/cch123/asm-cli)

Here is an example of it in action:

<script id="asciicast-sIksRB2w7zWKa17ruIkqVjOyI" src="https://asciinema.org/a/sIksRB2w7zWKa17ruIkqVjOyI.js" async></script>

Pretty useful if you want to determine the value a register has after a few instructions.

So far everything I have disassembled has been pretty basic code.

With the resources above, and through continued learning, I hope to be able to dive into more complex code.

I will be blogging about some more challenges soon hopefully.

I may make a post or two about xorpd's "xchg rax,rax" musings you can find on his website.