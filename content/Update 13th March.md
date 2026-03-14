---
date: 2026-03-13
author:
  name: RoosterBooster007
  url: https://github.com/RoosterBooster007
title: Update - 13th March 2026
---

### A Massive Foundation Shift

Welcome back! If you're looking at the numbers this week and thinking, "Only 15 PRs merged? Is the team sleeping?"—let me stop you right there. While our merge count might look a bit quieter this week, it's because we just landed an absolute behemoth of an update. We've been heavily focused on getting a massive core API change through the pipeline, and we currently have over 55+ PRs sitting in the queue undergoing rigorous review and testing (thanks for being patient, devs).

This week, we've been making sure that the foundational stuff is rock solid. And trust me, what we merged this week changes the game for Pumpkin entirely. 

### WebAssembly is Here!

The biggest news of the week: **We got WASM!** Our plugin API is officially migrating to WebAssembly. We made this major architectural shift primarily for two reasons: **improved compatibility and top-tier security**. By sandboxing plugins in WASM, we ensure that server owners have a much safer environment, and developers have a more flexible, cross-language compilation target.

A massive shout-out is owed to **BjornTheProgrammer**, who led the charge on this monumental task. He implemented the core WASM plugin API ([#1675](https://github.com/Pumpkin-MC/Pumpkin/pull/1675)), created a much cleaner API for registering WASM events ([#1838](https://github.com/Pumpkin-MC/Pumpkin/pull/1838)), and added the ability to register permissions for these new plugins ([#1841](https://github.com/Pumpkin-MC/Pumpkin/pull/1841)). His hard work has laid the groundwork for the future of Pumpkin plugins.

Other contributors are already jumping on board to flesh out this new ecosystem. illyrius666 quickly stepped in to add context and player APIs, giving developers the ability to use `get_data_folder` and `get_name` right out of the gate ([#1843](https://github.com/Pumpkin-MC/Pumpkin/pull/1843), [#1840](https://github.com/Pumpkin-MC/Pumpkin/pull/1840)). 

If you want to be one of the pioneers building on this new system, go read through our completely updated [Plugin API Documentation](https://docs.pumpkinmc.org/plugin-dev/introduction) to get started!

### Expanding the World

Even with the heavy API focus, we still made sure to sprinkle some new content into world generation. 

If you find yourself wandering through a desert, keep your eyes peeled—chocodev11 successfully implemented the Desert Pyramid structure ([#1815](https://github.com/Pumpkin-MC/Pumpkin/pull/1815)). To balance out the dry heat, I spent some time in the water and added the feature generation for underwater magma blocks ([#1747](https://github.com/Pumpkin-MC/Pumpkin/pull/1747)).

### Squashing Bugs and Polishing Mechanics

On the mechanical side of things, we knocked out a few annoying bugs that were hindering the vanilla feel of the server:

- **Redstone & Pistons:** GreenedDev was our resident redstone engineer this week. He fixed an issue where redstone wire would stubbornly stay activated when it shouldn't ([#1855](https://github.com/Pumpkin-MC/Pumpkin/pull/1855)) and corrected a bug that prevented pistons from unextending properly ([#1812](https://github.com/Pumpkin-MC/Pumpkin/pull/1812)). 
- **Combat & Equipment:** Have you ever broken a tool and noticed the server didn't quite react right? andreisugu fixed this by making sure the server broadcasts the proper `EntityStatus` when equipment breaks ([#1837](https://github.com/Pumpkin-MC/Pumpkin/pull/1837)), so you get that satisfying (or terrifying) visual and audio feedback.
- **Server Stability:** yuminstalljoe took care of some backend housekeeping by dropping the receiver correctly on console exit ([#1839](https://github.com/Pumpkin-MC/Pumpkin/pull/1839)), ensuring the server shuts down just a little bit more gracefully.

### Wrapping Up

Huge thanks to everyone who contributed this week, and an extra special shout-out to all the developers who are already diving in and trying out the new WASM plugin API early. It's a huge step forward for the project, and we couldn't do it without your testing and feedback. 

With 55+ PRs in the oven, next week is going to be wild. Have a great weekend, start reading those WASM docs, and I'll see you next time! 🧡