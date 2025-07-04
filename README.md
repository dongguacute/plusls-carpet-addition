# plusls carpet addition

[![Issues](https://img.shields.io/github/issues/Nyan-Work/plusls-carpet-addition?style=flat-square)](https://github.com/Nyan-Work/plusls-carpet-addition/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/Nyan-Work/plusls-carpet-addition?style=flat-square)](https://github.com/Nyan-Work/plusls-carpet-addition/pulls)
[![CI](https://img.shields.io/github/actions/workflow/status/Nyan-Work/plusls-carpet-addition/build.yml?label=Build&style=flat-square)](https://github.com/Nyan-Work/plusls-carpet-addition/actions/workflows/CI.yml)
[![Release](https://img.shields.io/github/v/release/Nyan-Work/plusls-carpet-addition?include_prereleases&style=flat-square)](https://github.com/Nyan-Work/plusls-carpet-addition/releases)
[![Github Release Downloads](https://img.shields.io/github/downloads/Nyan-Work/plusls-carpet-addition/total?label=Github%20Release%20Downloads&style=flat-square)](https://github.com/Nyan-Work/plusls-carpet-addition/releases)

## The project will be maintained in this repository until plusls back.
e
English | [中文](./README_ZH_CN.md)

❗Before reporting a problem, be sure to try the latest [beta version](https://github.com/Nyan-Work/plusls-carpet-addition/releases) to check if the problem still exists.

📌If you only want the PCA sync protocol and are not interested in other features, I recommend the lightweight [pca-protocol](https://github.com/Fallen-Breath/pca-protocol).

This is a [Carpet mod](https://github.com/gnembon/fabric-carpet) extension mod, a collection of carpet mod style useful tools and interesting features.

Operation command: `/pca`

## Dependencies

| Dependency | Link1                                                               | Link2                                              | Link3                                           |
|------------|---------------------------------------------------------------------|----------------------------------------------------|-------------------------------------------------|
| Carpet     | [CurseForge](https://www.curseforge.com/minecraft/mc-mods/carpet)   | [GitHub](https://github.com/gnembon/fabric-carpet) | [Modrinth](https://modrinth.com/mod/carpet)     |
| Fabric API | [CurseForge](https://www.curseforge.com/minecraft/mc-mods/fabric)   | [GitHub](https://github.com/FabricMC/fabric)       | [Modrinth](https://modrinth.com/mod/fabric-api) |
| MagicLib   | [CurseForge](https://www.curseforge.com/minecraft/mc-mods/magiclib) | [GitHub](https://github.com/Hendrix-Shen/MagicLib) | [Modrinth](https://modrinth.com/mod/magiclib)   |

## Rule List
## autoTrade
Use dispenser to auto trade with villager.

If EMERALD_BLOCK under the dispenser, it will trade once.

If DIAMOND_BLOCK under the dispenser, it will trade all.

Trade offer depend on redStone power.
- Categories: `Dispenser`, `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## avoidAnvilTooExpensive
Allow anvil level cost above 40 (If the client is not installed mod, it will be too expensive but can be used in practice).
- Categories: `Feature`, `Need Client`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## creativePlayerNoDirectKillArmorStand
Creative Player No Direct Kill ArmorStand.
- Categories: `Creative`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## dispenserCollectXp
Dispenser use bottle to collect xp.
- Categories: `Feature`, `Dispenser`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## dispenserFixIronGolem
Dispenser can fix iron golem.
- Categories: `Feature`, `Dispenser`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## emptyShulkerBoxStack
Empty shulker boxes stack

Empty shulker boxes can stack in a player's inventory or hand.

But empty shulker boxes will not stack in other inventories, such as chests or hoppers.
- Categories: `Feature`, `Need Client`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## flippingTotemOfUndying
Players can flip and rotate blocks when holding Totem Of Undying.

Doesn't cause block updates when rotated/flipped.

When Totem Of Undying in main hand,  offhand is empty will flip block.

When Totem Of Undying in main hand,  offhand is not empty, will place flipped block.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## forceRestock
Use spectral arrow to shoot villager to force restock.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## gravestone
place gravestone after player dead.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)

![player_dead.gif](./docs/player_dead.gif)
![break_gravestone.gif](./docs/break_gravestone.gif)
## pcaDebug
pcaDebug mode.
- Categories: `Debug`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## pcaSyncPlayerEntity
Which player entity can be sync.

NOBODY: nobody will be sync.

BOT: carpet bot will be sync.

OPS: carpet bot will be sync, and op can sync everyone's player entity data.

OPS_AND_SELF: carpet bot and self data will be sync, and op can sync everyone's player entity data.

EVERYONE: everyone's player entity will be sync.
- Categories: `Protocol`
- Type: `Enum`
- Default value: ops
- Options: `nobody`, `bot`, `ops`, `ops_and_self`, `everyone`
- Validators:
    - Enum(Case-sensitive)
## pcaSyncProtocol
Support sync entity and blockEntity from server.
- Categories: `Protocol`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## playerOperationLimiter
One tick player can place 2 block, insta break 1 block, can't do it at the same tick.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## playerSit
Player can sit down when fast sneak 3 times.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## potionRecycle
Dispenser can clear potion to cauldron.
- Categories: `Feature`, `Dispenser`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## powerfulBoneMeal
Allow use bone meal in cactus, sugar cane, chorus flower.
- Categories: `Feature`, `Dispenser`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## quickLeafDecay
quick leaf decay.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## renewableNetheriteEquip
Only in nether, throw the diamond equipment with 1 durability to lava fluid to get netherite equipment.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
- Dependencies:
    - And (All conditions need to be satisfied):
        - minecraft: >1.15.2

## sleepingDuringTheDay
World will switch to night when player sleep during the day.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## spawnBiome
spawn biome.
- Categories: `Feature`
- Type: `Enum`
- Default value: default
- Options: `default`, `desert`, `plains`, `the_end`, `nether_wastes`
- Validators:
    - Enum(Case-sensitive)
## spawnYMax
spawn Y Max, 114514 to close.
- Categories: `Feature`
- Type: `Integer`
- Default value: 114514
## spawnYMin
spawn Y Min, 114514 to close.
- Categories: `Feature`
- Type: `Integer`
- Default value: 114514
## superLead
Leash villagers and mobs by lead.
- Categories: `Feature`, `Need Client`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## trackItemPickupByPlayer
When item pick up by player, item will freeze.
- Categories: `Creative`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## useDyeOnShulkerBox
Dyes can be used on shulker boxes, empty potion will clean color.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## villagersAttractedByEmeraldBlock
Villagers are attracted by emerald block.
- Categories: `Feature`
- Type: `Boolean`
- Default value: false
- Options: `true`, `false`
- Validators:
    - Strict(Case-insensitive)
## xaeroWorldName
set xaero world name to sync word id to xaerominimap, "#none" is disable.
- Categories: `Protocol`
- Type: `String`
- Default value: #none
- Options: `#none`

## Development

### Support

Current main development for Minecraft version: 1.20.4

And use `preprocess` to be compatible with all versions.

**Note: We only accept the following versions of issues. Please note that this information is time-sensitive and any version of the issue not listed here will be closed**

- Minecraft 1.14.4
- Minecraft 1.15.2
- Minecraft 1.16.5
- Minecraft 1.17.1
- Minecraft 1.18.2
- Minecraft 1.19.2 (Ending support soon)
- Minecraft 1.19.3 (Ending support soon)
- Minecraft 1.19.4
- Minecraft 1.20.1 (Ending support soon)
- Minecraft 1.20.2 (Ending support soon)
- Minecraft 1.20.4

### Mappings

We are using the **Mojang official** mappings to de-obfuscate Minecraft and insert patches.

### Document

The English doc and the Chinese doc are aligned line by line.

## License

This project is available under the CC0-1.0 license. Feel free to learn from it and incorporate it in your own projects.
