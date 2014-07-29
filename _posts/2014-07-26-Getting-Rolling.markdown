---
layout: post
title: "Getting Rolling"
date: 2014-07-26 20:30:42
categories: Updates
---

It's been a busy week, but Project Otrera is moving along steadily. Here is a list of updates:

Recruiting:

Recruiting is going fairly well. I've got five guys who have expressed interest and one who has actually set up an IRC channel for the project on Freednode (#Otrera). Going to check it out this weekend. If I can start dolling out minor tasks based on people's interests and skillsets, I think development speed should see a huge boost.

Recruiting efforts will stay focused on 4chan and Reddit for now. This isn't exactly the Linux kernel; a small focused team even working only part-time should be able to complete Project Otrera in a matter of months.

Coding:

New features since the last update include a content editor module and a number of refactor commits. The former will allow for easy tweaking of existing content items in everything.json. This includes characters, classes, skills, - you name it. Version 0.0.1 will see all content in a single JSON file.

The refactors include some code cleanup and other improvements. I've added docstrings and comments in a number of places. I have tweaked a few classes and methods to make things more modular and flexible. The directory structure also now reflects the concepts of 'engines' and 'games', the latter being a subset of the former. Considering how busy I have been, it isn't bad for three days' work.

Other changes

I wrote this down as a github issue for the project but I'll briefly mention it here. There are two significant code changes I need to make in the coming days. Neither were planned; both are the result of some reflection on D&D.

The first and arguably simpler issue is that I need to simplify my objects. Character and skill objects probably don't need dictionary objects; if we can flatten them such that they only use strings, ints, and lists, it will make batch updates from CSV's much easier (among other things).

The second issue is that I think the default engine needs to be based more on Pathfinder. I don't think we need to copy D&D attribute names, or skills, or classes, but it needs to be complex enough to create a Pathfinder-style game. This refactor entails adding concepts like races, non-combat abilities, and feats to the character and leveling systems. This development will likely take place on a branch initially and be merged when complete.

The more general thing that has occurred to me is that 'engine-builder' is going to be a more complex module than I realized. Giving the user the ability to define everything from the ground up will involve a lot of decoupling of functionality (more JSON, less Python since the former is easier to programatically generate) and modularity.

This whole thing is going to be harder than I thought...
