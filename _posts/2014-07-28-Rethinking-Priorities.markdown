---
layout: post
title: "Rethinking Priorities"
date: 2014-07-28 21:23:11
categories: Updates
---

I haven't actually coded anything today. I may push a minor change to just to keep my github streak. I've slowed down over the last day both because I've been very busy with my day job and also because I've been doing a lot of thinking about my approach on this project.

Simply put, I think I need to change my priorities. For one, I don't think it makes sense to add "Pathfinder-level" complexity to the default engine. The default engine I think has enough features to be a default. What's more, I am going to encode Pathfinder's engine directly. There's no reason to make the default some weird knockoff.

I am also re-thinking my data model simplification. It may not be necessary. At least, I think it should be done in tandem with a higher priority task: Converting the default engine to JSON.

See, what I realized is that there is no point modifying the default engine in a way that will need to be re-coded when we start working on 'Engine Builder.' I already have a complete default engine and I already know how I am going to build 'Game Builder'; that'll just be a module taking user input to build a fresh "everything.json."

But before that I need to create an "engine.json." This is what 'Engine Builder' will create. You'll have one high-level master skeleton engine that loads modules based on the JSON engine definition.

This will require a lot more thinking about the precise distinction between 'Games' and 'Engines'. The edges between the two concepts are more blurred than I had originally realized. I'm going to need to do some whiteboarding and experimentation.

Anyway, my new sense of priorities is as follows:

Evaluate data model --> Convert default engine to JSON --> Create Game Builder --> Encode the Pathfinder engine --> Begin work on 'Engine Builder'. Some of this can be done in parallel and there are a number of subtasks and priorities. Fortunately, I have some help now and regular chunks of time to work at night.
