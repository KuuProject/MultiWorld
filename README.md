<a align="center"><img src="https://image.ibb.co/gPs5Se/Multi_World.png"></a>

<p align="center">
  <a href="https://www.paypal.com/donate/?hosted_button_id=SRQH6M2S6LV6Y;">
    <img src="https://img.shields.io/badge/donate-paypal-ff69b4?style=for-the-badge&logo=paypal">  
  </a>
  <a href="https://poggit.pmmp.io/ci/CzechPMDevs/MultiWorld/MultiWorld">  
    <img src="https://poggit.pmmp.io/ci.shield/CzechPMDevs/MultiWorld/MultiWorld?style=for-the-badge">  
  </a>  
  <a href="https://discord.gg/uwBf2jS">  
    <img src="https://img.shields.io/discord/365202594932719616.svg?style=for-the-badge&color=7289da&logo=discord&logoColor=white&logoWidth=12">  
  </a>
  <a href="https://poggit.pmmp.io/p/MultiWorld">  
    <img src="https://poggit.pmmp.io/shield.downloads/MultiWorld?style=for-the-badge">  
  </a> 
<br><br>
    ✔️ Passing PHPStan Level 9
    <br>
    ✔️ Simple world management commands
    <br>
    ✔️ Custom generators (Vanilla, Ender, Nether, Void, SkyBlock)
    <br>
    ✔️ Supports last PocketMine API version
    <br>
    ✔️ Multi-language system
    <br>
    ✔️ Simple API for other plugins
    <br>
    ✔️ Command autofill
    <br><br>
</p>

## 👍 2.0.0 Update:

> - Removed old Custom & Custom Nether generators
> - Added Muqsit's VanillaGenerator (Normal and Nether) with some modifications & fixes
> - Removed /mw update & /mw gamerule commands. There will be replacements for those in the future
> - Removed GameRules api
> - Removed Dimension handling api
> - Added command autofill with CortexPE's library Commando

## ⬇️ Downloads:

| Downloads                                         | API       | Downloads                                                                 |
|---------------------------------------------------|-----------|---------------------------------------------------------------------------|
| Latest Beta Release (2.1.0-beta2)                 | 5.x       | [Poggit](https://poggit.pmmp.io/r/211238/MultiWorld.phar)                 |
| Latest Stable Release (1.7.0)                     | 4.x       | [Poggit](https://poggit.pmmp.io/r/177396/MultiWorld.phar)                 |
| Latest Dev Build  (2.0.0 for 4.x / 2.1.0 for 5.x) | 4.x / 5.x | [Poggit CI](https://poggit.pmmp.io/ci/CzechPMDevs/MultiWorld/MultiWorld/) |
<br>

> **Other plugins by CzechPMDevs [here](https://poggit.pmmp.io/plugins/by/CzechPMDevs)**

<br>

## 📁 Supported software:

**This plugin works only on PocketMine-MP.** You can download [MultiWorld by Creeperface](https://github.com/Creeperface01/MultiWorld) for Nukkit or [MultiWorld by ferrybig](https://dev.bukkit.org/projects/multiworld-v-2-0) for Bukkit. **PMMP Spoons are NOT supported.**

## 🔧 How to install MultiWorld?

1) [Download](https://poggit.pmmp.io/p/MultiWorld) latest stable released version from poggit
2) Move dowloaded file to your server **/plugins/** folder
3) Restart the server

## 🌎 World management commands:

- All MultiWorld commands starts with `/mw` (`/multiworld`) except for the `/gamerule` command that was added as an alias to change game rules from settings.
- In game, you can get list of all commands using commands `/mw help`

<br>

**All MultiWorld Commands:**

| **Command**      | **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **/mw help**     | **Displays list of all MultiWorld commands** <br><br> Alias: `/mw ?` <br>Usage: `/mw help <page: 0-1>`                                                                                                                                                                                                                                                                                                                                              |
| **/mw create**   | **Generate new world using seed and generator** <br><br> Aliases: `/mw new`, `/mw generate` <br> Usage: `/mw create <levelName> [seed] [generator]` <br><br> Seed is value seed is the initial value by which the world is generated, when you set it empty, world will be generated by random number. You can use 6 generators (`Normal`, `Nether`, `End`, `Void`, `SkyBock` and `Nether_Old` = Nether generator without glowstone and quartz ore) |
| **/mw teleport** | **Teleports you or seleced player to world spawn** <br><br> Aliases: `/mw tp`, `/tp move` <br> Usage: `/mw tp <levelName> [player]` <br><br> If you are using [Slapper](https://poggit.pmmp.io/p/Slapper/) plugin and after you click on the npc you want to move the player to another world, you can use `/slapper edit <id> addcommand mw tp <world> {player}` command                                                                           |
| **/mw list**     | **Displays list of all levels** <br><br> Alias: `/mw ls` <br> Usage: `/mw list`                                                                                                                                                                                                                                                                                                                                                                     |
| **/mw info**     | **Displays level information** <br><br> Alias: `/mw i` <br> Usage: `/mw info` <br><br> This command can be used only in game                                                                                                                                                                                                                                                                                                                        |
| **/mw delete**   | **Remove level** <br><br> Aliases: `/mw del`, `/mw dl`, `/mw remove`, `/mw rm` <br>Usage: `/mw remove <level>` <br><br> Default level can not be deleted                                                                                                                                                                                                                                                                                            |
| **/mw load**     | **Loads level** <br><br> Aliases: `/mw ld` <br> Usage: `/mw load <level>`                                                                                                                                                                                                                                                                                                                                                                           |
| **/mw unload**   | **Unloads level** <br><br> Aliases: `/mw unld` <br> Usage: `/mw unload <level>`                                                                                                                                                                                                                                                                                                                                                                     |
| **/mw rename**   | **Renames level** <br><br>Aliases: `/mw rnm`, `/mw re` <br> Usage: `/mw rename <levelName> <newName>` <br><br> This command changes name of the folder and of nbt too.                                                                                                                                                                                                                                                                              |
| **/mw manage**   | **Opens world form manager** <br><br>Aliases: `/mw mng`, `/mw mg` <br> Usage: `/mw manage` <br><br> The form manager just dispatches command as a player, so player needs also permission for the command.                                                                                                                                                                                                                                          |
| **/mw setspawn** | **Updates world spawn** <br><br>Usage: `/mw setspawn`                                                                                                                                                                                                                                                                                                                                                                                               |
| **/mw setlobby** | **Updates server lobby** <br><br> Usage: `/mw setlobby`                                                                                                                                                                                                                                                                                                                                                                                             |

## ⛰️ Generators

### Custom World Generator:

<img src="https://github.com/CzechPMDevs/VanillaGenerator/blob/screenshots/screenshots/Forest%20biomes,%20Plains,%20River.png?raw=true">
<img src="https://github.com/CzechPMDevs/VanillaGenerator/blob/screenshots/screenshots/Ice%20Plains,%20Tundra.png?raw=true">
<img src="https://github.com/CzechPMDevs/VanillaGenerator/blob/screenshots/screenshots/Savanna%20Mountains.png?raw=true">
<img src="https://github.com/CzechPMDevs/VanillaGenerator/blob/screenshots/screenshots/Savanna.png?raw=true">
<img src="https://github.com/CzechPMDevs/VanillaGenerator/blob/screenshots/screenshots/Swamp,%20Mountains.png?raw=true">

###  Nether World Generator:
<img src="https://i.ibb.co/1KXb8FX/image.png">
<img src="https://i.ibb.co/xm05rDw/image.png">

### End World Generator:
<img src="https://i.ibb.co/G7rbRHp/image.png">
<img src="https://i.ibb.co/KsPPjrJ/image.png">

### SkyBlock Generator:
<img src="https://i.ibb.co/DDVM4zM/image.png">

## 🌐Add your language!

- Do you want to help with the development of MultiWorld? Add your native language!

1) Open [lanuage resource file](https://github.com/CzechPMDevs/MultiWorld/tree/master/resources/languages)
2) Click create new file
3) Translate e.g. language from English file https://github.com/CzechPMDevs/MultiWorld/blob/2.0.0/resources/languages/en_US.yml
4) Click Propose new file

## 💰 Credits

**Icon**
- Icon made by [Freepik](http://www.freepik.com/ "Freepik") from [www.flaticon.com](https://www.flaticon.com/ "Flaticon") is licensed by [CC 3.0 BY](http://creativecommons.org/licenses/by/3.0/ "Creative Commons BY 3.0")

**Vanilla (Overworld & Nether) generators**
- Generators translated from Glowstone project to PocketMine by @Muqsit

**Translations**
- Japanese translation by [fuyutsuki](https://github.com/fuyutsuki)
- Russian translation by [SteinsSquad (themestl)](https://github.com/themestl)
- Indonesian translation by [WooWBoom](https://github.com/GitWoow) and [keenanyafiqy](https://github.com/keenanyafiqy)
- German translation by [SchdowNVIDIA](https://github.com/SchdowNVIDIA) and [Tobikisss](https://github.com/Tobikisss)
- Chinese translation by [abc1460132901](https://github.com/abc1460132901) and [AZ1IDJC](https://github.com/Blackjack200)
- Vietnamese translation by [NhanAZ](https://github.com/NhanAZ)
- Spanish translation by [MrBlastyMSK](https://github.com/MrBlasyMSK)
- French translation by wrathx, [Hydros01](https://github.com/Hydros01)
- Thai translation by [KohakuChanX](https://github.com/Kuuuuuuuu)

##  💡 License

```
MultiWorld - PocketMine plugin that manages worlds.
Copyright (C) 2018 - 2023 CzechPMDevs

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <https://www.gnu.org/licenses/>.
```

Full license [here](https://github.com/CzechPMDevs/MultiWorld/blob/master/LICENSE).
