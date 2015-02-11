#TogglePvP

This plugin is based off of [pvpcontrol](http://dev.bukkit.org/bukkit-plugins/pvpcontrol/). However, that plugin was rather buggy and limited in it's features. This is an improvement.

###What it does

This plugin allows players to change their status from PvP to PvE and back again. It prevents almost any form of direct damage between players unless they are both set to PvP. This includes harmful and poison splash potions and arrows. **This plugin requires [iTag](http://www.spigotmc.org/threads/itag.11899/)**

###Plugin Features

- Colors players nameplate and their name on the TAB list based off their status
  - Red = PvP
  - Green = PvE
  
- Allows for PvP in the Nether and the End regardless of player status
  - These areas are meant to be more dangerous than the regular overworld, however you can disable this in the config
  
- Cool down timer so that players don't abuse changing their status to troll others

###Commands

- **/togglepvp (player)**
  - Switch back and forth between PvP and PvE
  - Cool down timer can be configured in the config.
  - Requires *togglepvp.player* to run on self or *togglepvp.admin* to run on another player
  - Aliases: **/tpvp**
  
- **/togglepvpreset**
  - Resets a players cool down timer
  - Requires *togglepvp.admin*
  - Aliases: **/tpvpr**
  
###Dependencies
- TogglePvP requires [iTag](http://www.spigotmc.org/threads/itag.11899/)
  
###Upcoming features

- I plan on adding a command to view remaining cool down time
- I'm currently working on a way for players with *togglepvp.admin* to use pvp whenever they want, despite their settings

###Known Issues

- Every once in a while, a player will not be removed from cooldown list when they should and have a negative remaining time.
- Using /togglepvp on another player does not appear to work when run from a sign with the plugin CommandSigns

### Misc

[Download link!](https://github.com/10becja/MinecraftPlugins/blob/master/TogglePvP/TogglePvP.jar?raw=true)  

[TogglePvP repository](https://github.com/10becja/TogglePvP)

Found a bug or want to request a feature? Please let me know [here!](https://github.com/10becja/TogglePvP/issues)

Come play minecraft with us at [play.minecraft.dk!](minecraft.dk)
