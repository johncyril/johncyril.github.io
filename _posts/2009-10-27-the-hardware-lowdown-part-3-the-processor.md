---
layout: post
title: "Hardware Lowdown: Part 3 - The Processor..."
date: 2009-10-27 22:22
author: admin
comments: true
categories: [Technology]
tags: [cpu, logic, logic gates, Moore's law, processor]
---
In what is likely to be the last of these hardware lowdown posts, we shall attempt to break-down the intricate world of the micro-processor. (aka CPU)

In the simplest of terms, the CPU on your computer is a fairly small chip that sits at the heart of the [motherboard](http://blog.johncyril.com/?p=61).
It's responsible for doing all the "thinking", "talking" and "fetching" of information between all other components in the computer, primarily your [hard disk](http://blog.johncyril.com/?p=75).

<!--more-->

[caption id="" align="alignright" width="300" caption="An early processor"]![An early processor](http://upload.wikimedia.org/wikipedia/commons/5/52/Intel_4004.jpg "early processor")[/caption]

... But how do they work? To explain this, I need to first talk a bit about logic. Some of you may think of logic as a fairly trivial and boring part of day to day life... When it comes to computers however (or your <a href="http://en.wikipedia.org/wiki/Sudoku" target="blank">Sudoku</a> on the train), there is nothing else you can use. Computers certainly have no intuition... I'm not yet sure whether there's intuition in sudoku or not...

Anyway. Logic. Let me start by making a few statements:
<p style="padding-left: 30px;">*"All cats are black"*

<p style="padding-left: 30px;">*"All black things are TVs"*

Stupid statements right? In fact, they are entirely "illogical" because we know them not to be true.
If however, you were to tell a computer that both these premises were true, the computer would come out with:
<p style="padding-left: 30px;">*"All cats are TVs"*

The computer doesn't have life experience. It doesn't *know* that my guitar case isn't a TV.. or that your cat isn't a TV. It only goes by what you told it to be "true". It *assumes* that what you tell it is true, unless you explicitly tell it something is false... Yes. Computers are stupid.

I'd like to note, that this is intentionally a non-mathematical example.. Your computer, well namely the CPU, only talks in numbers. And, it would only give you a true or false for a statement.

A computer would be given a "mathsey" version of this:
<p style="padding-left: 30px;">*"All cats are black AND all black things are televisions THEREFORE all cats are televisions"*

The words in capital letters are key in the processing of the statement..

When processed, the computer will give either "True" or "False"... True in this case. To explain why, is to dive into something called <a href="http://en.wikipedia.org/wiki/Propositional_calculus" target="blank">Propositional logic</a> and <a href="http://en.wikipedia.org/wiki/Transitive_relation" target="blank">transitivity</a>. Very interesting stuff but beyond the scope of this post.

What I will say is, think of each of the capital words above as a gate. A [logic gate](http://en.wikipedia.org/wiki/Logic_gates). Each logic gate has rules that "weigh-up" the statements either side of it and either "permit" or "deny"... in other words deem *true *or *false. *
The AND gate for example will only deem *true* if <span style="text-decoration: underline;">both</span> statements either side are true.
So if you could tell the processor:
<p style="padding-left: 30px;">*"All cats are black AND All dogs are green"*

It would say *true*.
<p style="padding-left: 30px;">*"All cats are black AND **not all cats are black"*

Would bring *false*..

This makes sense to anyone really.. Something cannot be true and false at the same time.
These logic gates can be physically made using electronic components called transistors. There are AND gates and OR gates and NAND gates... and a few others..

If you asked your computer to find your coursework, it would go about it along the following simplified lines...

"is it here?" no. change location. "changed location". "is it here?" no. change location. "changed location". "is it here?"......
till it gets a yes.

All these are logical steps in the processor, and go through at the very, VERY least one logic gate made up of many transistors.
The speed of your CPU is measured by how many of those transistors are inside of it. When they first started, microprocessors had only a few hundred transistors. Today, a single chip has a hundreds of millions...

These little chips are probably the fastest evolving components in today's computer systems. There is this interesting idea called "<a href="http://en.wikipedia.org/wiki/Moores_law" target="blank">Moore's law</a>"... Basically, it suggests the amount of transistors you can cram into a chip should double within 18-24 months..

Mad...
