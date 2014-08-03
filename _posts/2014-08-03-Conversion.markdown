---
layout: post
title: "Conversion"
date: 2014-08-03 12:10:32
categories: Plans
---

Converting the original game engine from Python to JSON has proved an amusing challenge over the last few days. I am in the final stretch now dealing with skill objects. These are difficult structures to work with as they contain a lot of information, much of it not easily quantified and related.

I've found a "good enough" solution for the structure and for dependency mapping. I can prompt users for the needed info to programatically generate JSON that establishes dependencies between things like character class and skills or equipment. Once I work out the bugs and get the complete character builder program working again, I'll be at a significant milestone.

The idea that a table top game can be represented in a structured data format like JSON is not especially radical (or even new I suspect) but it is the foundation of the service Otrera will provide. Once you have that output, you can build all sorts of tooling around it. Programs to edit or generate new games. Analytical programs. Visualizations. There's a lot I'm probably not even thinking of.

Otrera's priority is just getting that output. This is the goal of 'Engine Builder' - let me start with an idea in my head, and end with a blob of JSON that represents my idea made manifest. From there, the sky is the limit. My thinking is that the analytics, visualization, and other pieces will be separate libraries that plug into an Otrera API.

But that's all getting ahead of myself. While I am excited about adding all sorts of cool features and doing Kickstarter, my priority now is Game Builder. I have a number of tasks to complete to make that real, including integration tests, code cleanup, and documentation. I still think I can get it done by 8/8, which was the goal on the ROADMAP.
