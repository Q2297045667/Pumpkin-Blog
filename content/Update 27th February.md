---
date: 2026-02-27
author:
  name: RoosterBooster007
  url: https://github.com/RoosterBooster007
title: Update - 27th February 2026
---

### Quality Over Quantity (But Still Plenty!)

Hey everyone, RB007 here again. If you’ve been watching our GitHub pulse, you might have noticed the numbers looked a little different this week. We merged **32 pull requests**—which, while slightly lower than our usual "40-something" madness, definitely doesn't mean we're slowing down. 

In fact, the "kitchen" is currently overflowing. We have a **massive** number of PRs currently in the works, undergoing heavy review, or being polished to perfection. Sometimes you have to slow down the "merge" button to make sure the big features land softly. That said, what *did* get into the main branch this week is still pretty beefy. Let’s take a look.

### Smarter Mobs & Complex Commands

The world of Pumpkin is getting better and more "vanilla" by the second. 

- **Endermen & Pigs**: Purdze is back at it with more AI! Endermen are now teleporting around (watch your eyes) and Pigs have officially joined the livestock roster ([#1579](https://github.com/Pumpkin-MC/Pumpkin/pull/1579), [#1593](https://github.com/Pumpkin-MC/Pumpkin/pull/1593)).
- **The Command Overhaul**: Laptop59 has implemented a brand-new command system ([#1681](https://github.com/Pumpkin-MC/Pumpkin/pull/1681)). This is a huge internal shift that allows us to handle the complex, nested arguments you see in vanilla Minecraft. It’s the groundwork for making things like `/execute` feasible to recreate.
- **Monitoring Performance**: We’ve added a `/tps` command so you can see exactly how smooth the Rust engine is purring ([#1669](https://github.com/Pumpkin-MC/Pumpkin/pull/1669)).

### Support for More Java Edition Versions

We also extended Java Edition protocol support (>=1.21) in [#1435](https://github.com/Pumpkin-MC/Pumpkin/pull/1435), thanks to topi-banana. This required a large refactor for multi-version packet support and advanced remappings.

### A World of Color (and Language)

We’ve had a massive surge in international support this week. It is genuinely awesome to see the community making Pumpkin accessible to everyone. We added more support for **German, Dutch, Albanian, Korean, Romanian, and Traditional Chinese** ([#1629](https://github.com/Pumpkin-MC/Pumpkin/pull/1629), [#1728](https://github.com/Pumpkin-MC/Pumpkin/pull/1728), [#1724](https://github.com/Pumpkin-MC/Pumpkin/pull/1724), etc.).

On the flora side of things:
- **Nether**: Crimson and Warped Fungus blocks are now implemented ([#1693](https://github.com/Pumpkin-MC/Pumpkin/pull/1693) - GreenedDev).
- **Ocean & More**: Kelp (generation) and Wither Roses are improved ([#1717](https://github.com/Pumpkin-MC/Pumpkin/pull/1717), [#1692](https://github.com/Pumpkin-MC/Pumpkin/pull/1692)).

### The "Little Things" That Matter

You know that annoying flicker when you break a block? Or when the sun doesn't quite move right? We spent a lot of time this week on the "feel" of the server:

- **Attributes & Effects**: I added an entity attribute system and fixed over a dozen status effects. Mobs now have unique health/speed traits, and effects like Invisibility and Glowing actually work ([#1526](https://github.com/Pumpkin-MC/Pumpkin/pull/1526)).
- **Visual Polish**: BraveDevelopment fixed the block-break flickering ([#1683](https://github.com/Pumpkin-MC/Pumpkin/pull/1683)), and I pushed a fix for the visual daylight cycle so the sun actually follows the timeline correctly ([#1684](https://github.com/Pumpkin-MC/Pumpkin/pull/1684)).
- **Physics Fixes**: Laptop59 made sure falling blocks keep their state (no more weird resets mid-air) and ensured Armor Stands actually respect gravity ([#1757](https://github.com/Pumpkin-MC/Pumpkin/pull/1757), [#1689](https://github.com/Pumpkin-MC/Pumpkin/pull/1689)).
- **Better Bed Behavior**: gula00 fixed the obstruction check so it now accurately checks both the head and foot of the bed. They also added a safety guard to ensure that breaking one half of a bed doesn't accidentally "eat" a non-bed block next to it—super helpful for those weird "half-bed" states ([#1696](https://github.com/Pumpkin-MC/Pumpkin/pull/1696)).
- **Spectator Logic**: kyotuca made sure spectators can no longer "accidentally" hoover up items like some kind of ghost-vacuum ([#1699](https://github.com/Pumpkin-MC/Pumpkin/pull/1699)).

### For the Developers: More Events!

Our plugin API is growing fast. yunuservices added a whole suite of new events for developers to hook into, including **Fishing, Experience Changes, Main Hand Swaps, Item Holding, and Spawn Changes** ([#1654](https://github.com/Pumpkin-MC/Pumpkin/pull/1654), [#1653](https://github.com/Pumpkin-MC/Pumpkin/pull/1653), [#1647](https://github.com/Pumpkin-MC/Pumpkin/pull/1647), etc.). If you’re building on Pumpkin, your toolbox just got a lot bigger. And, it'll continue to grow over the coming weeks as more features and events are added.

### Smoother Deployments with Pterodactyl

For those of you hosting Pumpkin on panels like Pterodactyl or Pelican, deployment just got a whole lot smoother thanks to vyPal ([#1498](https://github.com/Pumpkin-MC/Pumpkin/pull/1498)). 

Rust is a powerhouse, but it can be hungry during the compilation phase. We’ve updated our "egg" configuration to recommend 4GB of RAM (up from 2GB) to prevent build failures. We've also added recommendations for CPU limits and refined how Cargo build jobs are handled to make sure your server compiles as fast as possible.

### Wrapping Up

While 32 PRs might look like a "quiet" week compared to our usual breakneck speed, the reality is that the team is deep in the trenches on some of the most complex parts of the engine. There is a mountain of code currently being reviewed that we can't wait to show you.

Thanks for sticking with us and for all the feedback on the Discord. It’s been a blast seeing you test our latest changes. And to anyone who contributed this week: thank you! Y'all are helping push Pumpkin forward. 💕

Stay tuned for next week!