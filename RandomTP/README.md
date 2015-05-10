# RandomTP

Spawn area too crowded? Map too big to reach undeveloped areas? You need RandomTP!

###What it does

RandomTP will allow players to be randomly teleported somewhere on the map. This can be done either via command, or the first time a player joins a world. It curently requires [GriefPrevention](http://dev.bukkit.org/bukkit-plugins/grief-prevention/). The plugin makes sure that a player doesn't get teleported somewhere in the middle of a claim.

###Config

It's very important to configure this plugin, otherwise it won't work. 
- To start, drop it in your plugins folder and start up your server. You'll notice that RandomTP will warn you that it won't teleport new players.
- If you want to have new players be teleported on joining, change the *World:* entry in RandomTP/config.yml to the name of the world you want it to check for. RandomTP currently only supports one "first join" world
  - if you don't want players to be teleported when they join, just leave it.
- Another important step is to change the *Border:* entry. If you don't set this, your map will be HUGE.
- The last important step is to set the starting point. You can do this ingame by standing somewhere on your map (usually your original spawn point), and running **/tprs**. This will set the center of the search algorithm
- The other config options are fairly self explanatory. 


###Commands
- **/tpr (player)**
  - Teleport yourself or another player to a random location. 
  - Requires *randomtp.player* to teleport yourself and *randomtp.admin* to teleport someone else
  - aliases: **/tprrand, /randomtp, /tprrandom**

- **/tprs**
  - Sets the starting location for the search algorithm
  - Requires *randomtp.admin*
  - aliases: **/tprspawn, /randomtpspawn**
  
- **/tprb**
  - Returns you to your last random teleport spot
  - Requires *randomtp.back*
  - aliases: **/tprback, /randomtpback**


###Misc
[Download link!](https://github.com/10becja/MinecraftPlugins/raw/master/RandomTP/RandomTP.jar)

[RandomTP repository](https://github.com/10becja/RandomTP)

Found an issue or want to request a feature? Let me know [here!](https://github.com/10becja/RandomTP/issues)

Come play minecraft with us at [play.minecraft.dk!](minecraft.dk)
