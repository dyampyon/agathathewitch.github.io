---
layout: post
title: "The Way Forward"
date: 2014-07-30 16:14:35
categories: Plans
---

I have made some good progress on Otrera's code and feel confident that "Game Builder" will be done within a week. Already I have begun converting the Python engine modules to programatically creatable JSON, and so far the character builder modules work fine with it. My focus for the next few days is to just go heads down and keep hacking until that milestone is reached.

Once I hit that milestone I can take a step back and start thinking about "Engine Builder" and "Analytics." Part of me thinks that the latter will have to be a separate library or product that just works with Otrera's output JSON files. The scope of the Analytics project is unclear.

Engines should be just one big 'engine.json' file in a properly named directory. Subdirectories are named after games, which each have their own 'content.json' file that defines game elements. Engines are the more flexible construct; you should be able to create an 'engine.json' file that is essentially both an engine and a game, as engine.json files can contain content keys.

The reason for this flexibility is to allow for one-off engines. This is an extremely important use-case for developers. Not everyone wants their game engine to be general purpose. Many people might want their engine to be unique to only their one game. In effect, the game and the engine are then one and the same. This is something the Engine Builder module will have to support and properly communicate to the user.

The good news is that I feel more confident than I did a few days ago. In my head I can already see how to code all of this up. It will take several weeks to get it right, even if I work full-time. That doesn't even begin to address the complexity of making a better UI.

The more I think about it, the more Kickstarter seems like a good idea. I need to do some planning before I can do it though. I'd have to make a video, make a little test frontend with Game Builder, maybe have a separate logo, etc. etc. But I think this project is the sort of thing that people in the Kickstarter community in particular would get behind, as there are a lot of game builders on there.

More on all that later. Right now: Gotta code. 
