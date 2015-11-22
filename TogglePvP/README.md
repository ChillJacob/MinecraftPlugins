#TogglePvP

This plugin is based off of [pvpcontrol](http://dev.bukkit.org/bukkit-plugins/pvpcontrol/). However, that plugin was rather buggy and limited in it's features. This is an improvement.

###What it does

This plugin allows players to change their status from PvP to PvE and back again. It prevents almost any form of direct damage between players unless they are both set to PvP. This includes harmful and poison splash potions and arrows.

###Plugin Features

- Colors players nameplate and their name on the TAB list based off their status
  - Red = PvP
  - Green = PvE
  - You can customize the color in the config
  
- Allows for PvP in the Nether and the End regardless of player status
  - These areas are meant to be more dangerous than the regular overworld, however you can disable this in the config
  
- Cool down timer so that players don't abuse changing their status to troll others

###Commands

[] are optional, &lt;&gt; are required.

- **/togglepvp [player]**
  - Switch back and forth between PvP and PvE
  - Cool down timer can be configured in the config.
  - Requires *togglepvp.player* to run on self or *togglepvp.admin* to run on another player
  - Aliases: **/tpvp**
  
- **/togglepvpreset &lt;player&gt;**
  - Resets a players cool down timer
  - Requires *togglepvp.admin*
  - Aliases: **/tpvpr**
  
- **/togglepvpcheck [player]**
  - Used to manually check a players status
  - Requires *togglepvp.player* to use it on yourself, and *togglepvp.check* to use it on others
  - Aliases: **/check**, **/tpvpc**
  
- **/togglepvptime [player|list]**
  - This shows how much time is remaining before you can toggle again
  - Players with *togglepvp.admin* can use the **list** argument to view a list of everyone with a timer
  - Requires *togglepvp.player* to use it on yourself, and *togglepvp.admin* to use it on others
  - Aliases: **/tpvpt**, **/tpvptime** 

- **/lockpvp &lt;player&gt; &lt;true|false&gt;**
  - Requires *togglepvp.lock* permission
  - Allows you to lock a player in PvP or PvE mode
  - Can be used on offline players.

- **/unlockpvp &lt;player&gt;**
  - Also requires *togglepvp.lock*
  - Unlocks a players status and allows them to toggle again

###Permissions

Permissions needed for commands are listed above.

- *togglepvp.admin*
  - In addition to the commands above, this permission also allows the player to damage anyone, regardless of their status

### Misc

[Download link!](https://github.com/10becja/MinecraftPlugins/raw/master/TogglePvP/TogglePvP.jar)  

[TogglePvP repository](https://github.com/10becja/TogglePvP)

Found a bug or want to request a feature? Please let me know [here!](https://github.com/10becja/TogglePvP/issues)

Come play minecraft with us at [play.minecraft.dk!](minecraft.dk)
