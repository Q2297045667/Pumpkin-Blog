---
date: 2026-05-06
author:
  name: Missing_Love
  url: https://github.com/Q2297045667
title: Update - 6th May 2026
---


### Pumpkin Development Update - Alpha Release Approaching

Hello everyone, this is Missing_Love. It has been quite some time since our last blog post. This delay is not due to any difficulties with Pumpkin, nor does it indicate that we are abandoning the project. On the contrary, we are approaching our first Alpha release aimed at developers. Recently, our team has been intensively working on stabilizing Pumpkin and enhancing its API...

## Port to 26.1

### AI Updates
- **WhiteProject1** [#1794](https://github.com/Pumpkin-MC/Pumpkin/pull/1794) optimized the **pathfinding system**
- **Alex** fixed **mob pathfinding jump** mechanics and implemented **Villager trading** functionality along with all missing **entities**
- **RoosterBooster007** contributed the **Shulker entity and AI** [#2061](https://github.com/Pumpkin-MC/Pumpkin/pull/2061)
- **Alex** implemented **Blaze** and **Ender Dragon AI**

### Command System
- **Laptop59** [#1924](https://github.com/Pumpkin-MC/Pumpkin/pull/1924), [#1967](https://github.com/Pumpkin-MC/Pumpkin/pull/1967), [#1968](https://github.com/Pumpkin-MC/Pumpkin/pull/1968), [#1969](https://github.com/Pumpkin-MC/Pumpkin/pull/1969), [#2050](https://github.com/Pumpkin-MC/Pumpkin/pull/2050) and **SomeYellowGuy** [#1700](https://github.com/Pumpkin-MC/Pumpkin/pull/1700), [#1918](https://github.com/Pumpkin-MC/Pumpkin/pull/1918), [#1919](https://github.com/Pumpkin-MC/Pumpkin/pull/1919), [#1971](https://github.com/Pumpkin-MC/Pumpkin/pull/1971) have migrated numerous commands to the new command system
- **SomeYellowGuy** [#1925](https://github.com/Pumpkin-MC/Pumpkin/pull/1925), [#1943](https://github.com/Pumpkin-MC/Pumpkin/pull/1943), [#1994](https://github.com/Pumpkin-MC/Pumpkin/pull/1994), [#2001](https://github.com/Pumpkin-MC/Pumpkin/pull/2001), [#2004](https://github.com/Pumpkin-MC/Pumpkin/pull/2004), [#2005](https://github.com/Pumpkin-MC/Pumpkin/pull/2005), [#2038](https://github.com/Pumpkin-MC/Pumpkin/pull/2038), **Laptop59** [#2088](https://github.com/Pumpkin-MC/Pumpkin/pull/2088), and **vyPal** [#2076](https://github.com/Pumpkin-MC/Pumpkin/pull/2076) have significantly expanded the functionality of our new command system


### Chunk Improvements
- **Alex** finally resolved the long-standing **Chunk deadlock** issue that has plagued Pumpkin for years and added **canyon carvers**. We now have our own **Pumpkin format**
- We now have our own **PNBT** implementation with significant performance improvements, and the **linear format** has been updated from v1 to v2
- **andreisugu** [#1883](https://github.com/Pumpkin-MC/Pumpkin/pull/1883), [#1888](https://github.com/Pumpkin-MC/Pumpkin/pull/1888) optimized our chunk data packets, reducing unnecessary data transmission, eliminating DAG deadlocks, and greatly improving structure optimization
- **GreenedDev** [#1894](https://github.com/Pumpkin-MC/Pumpkin/pull/1894), [#1895](https://github.com/Pumpkin-MC/Pumpkin/pull/1895), [#2009](https://github.com/Pumpkin-MC/Pumpkin/pull/2009), [#2007](https://github.com/Pumpkin-MC/Pumpkin/pull/2007) and **RoosterBooster007** [#1879](https://github.com/Pumpkin-MC/Pumpkin/pull/1879), [#1887](https://github.com/Pumpkin-MC/Pumpkin/pull/1887), [#1886](https://github.com/Pumpkin-MC/Pumpkin/pull/1886), [#1885](https://github.com/Pumpkin-MC/Pumpkin/pull/1885), [#1884](https://github.com/Pumpkin-MC/Pumpkin/pull/1884), [#1882](https://github.com/Pumpkin-MC/Pumpkin/pull/1882), [#1890](https://github.com/Pumpkin-MC/Pumpkin/pull/1890) have made world generation more vibrant

### Bedrock Edition Support
Recent efforts have focused on extensive **Bedrock** compatibility work, enabling players to enjoy a more stable experience on Bedrock Edition.

### Wasm API Enhancements
- **yunuservices** [#1880](https://github.com/Pumpkin-MC/Pumpkin/pull/1880), [#1881](https://github.com/Pumpkin-MC/Pumpkin/pull/1881), [#1860](https://github.com/Pumpkin-MC/Pumpkin/pull/1860), [#1889](https://github.com/Pumpkin-MC/Pumpkin/pull/1889), [#1895](https://github.com/Pumpkin-MC/Pumpkin/pull/1895), [#1896](https://github.com/Pumpkin-MC/Pumpkin/pull/1896), [#1998](https://github.com/Pumpkin-MC/Pumpkin/pull/1998), [#1899](https://github.com/Pumpkin-MC/Pumpkin/pull/1899), **Laptop59** [#1988](https://github.com/Pumpkin-MC/Pumpkin/pull/1988), **TsubakiDev** [#1898](https://github.com/Pumpkin-MC/Pumpkin/pull/1898), [#1921](https://github.com/Pumpkin-MC/Pumpkin/pull/1921), **Alex**, and **vyPal** [#2077](https://github.com/Pumpkin-MC/Pumpkin/pull/2077) have contributed numerous **Wasm API** additions
- **Alex** implemented a more secure **plugin permission system** and **schedulers**
- **StormLight14** and **stormyyy** added fine-grained player permission control to the plugin API [#2059](https://github.com/Pumpkin-MC/Pumpkin/pull/2059)
- **QuantumSegfault** reworked the versioning logic in the Wasm plugin loader [#2046](https://github.com/Pumpkin-MC/Pumpkin/pull/2046)

### Structure Generation
- **GreenedDev** added **jungle temple** structure [#2054](https://github.com/Pumpkin-MC/Pumpkin/pull/2054)


These recent updates demonstrate our commitment to delivering a robust and feature-complete Minecraft server implementation. The Alpha release is approaching rapidly, and we appreciate the continued support from our community!