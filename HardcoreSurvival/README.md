#HardcoreSurvival

Regular survival too boring for you? Try this out!

This plugin is meant to emulate minecraft's hardcore mode. Normal hardcore is a bit cumbersome to use in a server environment. If a server administrator decided to allow someone to join again, they'd have to shut the entire server down to delete the player files. With this plugin, they simply need to unban the player.

Developed for a [server](minecraft.dk) running [GriefPrevention](http://dev.bukkit.org/bukkit-plugins/grief-prevention/), when a player dies they are forced to run **/abandonallclaims**. The idea behind this is that it will allow other players to loot their items and such.

Another feature of this plugin is that it alters the way the compass works.
- Right clicking with a compass will have it point towards the nearest player's location at the time of the click
- Left clicking will point the compass towards the player's base (explained further down) or where they spawned at.

This allows for the server to be even more challenging by not allowing players to teleport or /home and such.

[Optional Download](https://github.com/10becja/MinecraftPlugins/raw/master/HardcoreSurvival/HardcoreSurvivalListener.jar) This addon can be used to alert players on other servers (using bungee) that a player has died. It requires [CommandSync](http://www.spigotmc.org/resources/commandsync.115/) to run.

### Commands
HardcoreSurvival only has one command associated with it
- **/setbase**
  - This will store the players currently location as their base, which they can then use the compass to find again
  - Requires *hardcore.setbase* permission.
- **/hardcorereload**
  - Reloads the plugins configuration without having to restart the server
  - Requires *hardcore.reload* permission.
  - Aliases: /hcr
  
### Other permissions
- *hardcore.noban*
  - This allows players to be able to die without being banned.
- *hardcore.notrack*
  - Prevents a player from being tracked with compasses.
  
###Misc
[Download link!](https://github.com/10becja/MinecraftPlugins/raw/master/HardcoreSurvival/HardcoreSurvival.jar)

[HardcoreSurvival repository](https://github.com/10becja/HardcoreSurvival)

Found an issue or want to request a feature? Let me know [here!](https://github.com/10becja/HardcoreSurvival/issues)

Come play minecraft with us at [play.minecraft.dk!](minecraft.dk)
