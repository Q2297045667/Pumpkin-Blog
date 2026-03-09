---
date: 2026-03-06
author:
  name: RoosterBooster007
  url: https://github.com/RoosterBooster007
title: Update - 6th March 2026
---

### Stepping Closer to Vanilla

Hey everyone! It’s RB, back again to showcase some of the cool recent changes to hit Pumpkin. We've been hard at work merging 40+ pull requests this week, and while the numbers are a bit more focused, the impact on gameplay is massive. We are really starting to bridge the gap between our engine and the vanilla Minecraft experience.

Before we dive into the details, I highly recommend checking out our newest update video. It covers a lot of the changes we've made recently, and it really puts into perspective how fast things are moving. Give it a watch, like, and subscribe!

<Youtube videoId="GSaDNkqClZ8"></Youtube>

### Bringing the World to Life

World generation got a massive boost this week thanks to mtthidoteu. He implemented a brand new system to handle NBT templates for structures ([#1630](https://github.com/Pumpkin-MC/Pumpkin/pull/1630)). This is a huge deal because it makes porting certain structures over from vanilla significantly easier. Using this new system, he immediately added generation for Igloos and Nether Fossils ([#1631](https://github.com/Pumpkin-MC/Pumpkin/pull/1631), [#1632](https://github.com/Pumpkin-MC/Pumpkin/pull/1632)). 

I also wanted to jump in and help with worldgen, so I wrote up the feature generation code for Geodes and Monster Rooms/Dungeons ([#1697](https://github.com/Pumpkin-MC/Pumpkin/pull/1697), [#1748](https://github.com/Pumpkin-MC/Pumpkin/pull/1748)). On top of that, we finally tracked down and fixed that nasty Nether Portal crash ([#1710](https://github.com/Pumpkin-MC/Pumpkin/pull/1710)), so you can safely traverse dimensions again!

Last but not least, Purdze and Alex added Nether Fortresses into the mix, improving Stronghold generation in the process.

### Blocks, Blocks, and More Blocks

GreenedDev was on an absolute roll this week, bringing a ton of new blocks into the fold. He implemented all types of Lanterns, Copper Torches, Spore Blossoms, and Nether Sprouts ([#1779](https://github.com/Pumpkin-MC/Pumpkin/pull/1779), [#1772](https://github.com/Pumpkin-MC/Pumpkin/pull/1772), [#1735](https://github.com/Pumpkin-MC/Pumpkin/pull/1735), [#1736](https://github.com/Pumpkin-MC/Pumpkin/pull/1736)). But he didn't stop at just adding things; he also fixed a slew of block behaviors. For example, conduits will no longer be forced into a waterlogged state out of nowhere, piston break checks are fixed, and torch block-updates are properly aligned ([#1808](https://github.com/Pumpkin-MC/Pumpkin/pull/1808), [#1787](https://github.com/Pumpkin-MC/Pumpkin/pull/1787), [#1778](https://github.com/Pumpkin-MC/Pumpkin/pull/1778)).

Other contributors made huge strides in world interaction, too. Rotstein007 added vanilla powder snow behavior, meaning you’ll now take freezing damage when submerged—so watch your step ([#1743](https://github.com/Pumpkin-MC/Pumpkin/pull/1743))! LuciCrack introduced Daylight Detectors, making them successfully output a redstone signal based on the time of day ([#1596](https://github.com/Pumpkin-MC/Pumpkin/pull/1596)). Finally, yuminstalljoe fixed tall plants so they properly place their upper halves when planted, and made sure lava correctly flows when placed above a water block ([#1738](https://github.com/Pumpkin-MC/Pumpkin/pull/1738), [#1737](https://github.com/Pumpkin-MC/Pumpkin/pull/1737)).

### Mechanics and Under-the-Hood Polish

If you enjoy smacking zombies around, you'll be happy to know that LegendsOfXania added mob sunburn ([#1767](https://github.com/Pumpkin-MC/Pumpkin/pull/1767)). Undead mobs will now rightfully burn to a crisp during the day. Speaking of entities, yuminstalljoe fixed an issue where dying entities weren't ticking for movement, meaning they now take knockback in death as expected (though they still seem to pathfind for those 20 extra ticks), and he aligned entity water velocity with Java Edition ([#1741](https://github.com/Pumpkin-MC/Pumpkin/pull/1741), [#1739](https://github.com/Pumpkin-MC/Pumpkin/pull/1739)).

We also squashed a few annoying bugs regarding player mechanics. WCBBEX implemented the `natural_regeneration` gamerule check directly into the hunger manager ([#1764](https://github.com/Pumpkin-MC/Pumpkin/pull/1764)). GroobleDierne swept in to fix some boss bar encoding issues alongside a few effects bugs ([#1766](https://github.com/Pumpkin-MC/Pumpkin/pull/1766)), and chocodev11 fixed an annoying bug where using rotation arguments in a `/tp` command would aggressively force you back into the Overworld ([#1690](https://github.com/Pumpkin-MC/Pumpkin/pull/1690)).

### Expanding the Developer Toolbox

Yunuservices has been steadily tackling the massive task of implementing Bukkit-style events. This week, we got `PlayerEggThrowEvent`, `BlockGrowEvent` for crops, and `BlockRedstoneEvent` for pressure plates ([#1753](https://github.com/Pumpkin-MC/Pumpkin/pull/1753), [#1752](https://github.com/Pumpkin-MC/Pumpkin/pull/1752), [#1750](https://github.com/Pumpkin-MC/Pumpkin/pull/1750)).

On the data and documentation side, SomeYellowGuy added wrapping and unwrapping for NBT lists to and from binary ([#1742](https://github.com/Pumpkin-MC/Pumpkin/pull/1742)). HairlessVillager refactored the `PalettedContainer` for better performance and corrected Y-coordinate checks in light propagation ([#1721](https://github.com/Pumpkin-MC/Pumpkin/pull/1721), [#1791](https://github.com/Pumpkin-MC/Pumpkin/pull/1791)). And because good documentation is the lifeblood of open source, illyrius666 added thorough docs to `pumpkin-macros` and `pumpkin-util` ([#1720](https://github.com/Pumpkin-MC/Pumpkin/pull/1720), [#1719](https://github.com/Pumpkin-MC/Pumpkin/pull/1719)).

### A Global Community

We continue to get a ton of love from translators! This week, we expanded our `/pumpkin` command support with Plattdüütsch (nds_de), Polish (pl_PL), Breton (brb), Italian (it_it), and Georgian (ka_ge) ([#1763](https://github.com/Pumpkin-MC/Pumpkin/pull/1763), [#1776](https://github.com/Pumpkin-MC/Pumpkin/pull/1776), [#1727](https://github.com/Pumpkin-MC/Pumpkin/pull/1727), [#1718](https://github.com/Pumpkin-MC/Pumpkin/pull/1718), [#1625](https://github.com/Pumpkin-MC/Pumpkin/pull/1625)). While adding translations works fine on GitHub for now, we’re thinking of moving it to a platform like Crowdin for simplicity soon. Stay tuned for updates on that front.

### Wrapping Up

Overall, we’re succeeding in our quest to make Pumpkin the best custom Minecraft server software out there. And speaking of a "quest," Pumpkin was recently spotted running natively on a Meta Quest 2, which is absolutely wild and shows off just how flexible and performant this software is... and how creative our community can be!

I personally love seeing all of your fixes and new features pour in. We’re incredibly grateful to everyone who has contributed to or supported Pumpkin in any way.

See you next time! Thank you all for making this possible! 🧡