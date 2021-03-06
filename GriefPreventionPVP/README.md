# GriefPreventionPVP

This is a fork of the plugin [GriefPrevention](http://dev.bukkit.org/bukkit-plugins/grief-prevention/) by [RyanHampshire](https://github.com/ryanhamshire)

GriefPreventionPvP adds several new commands which enhance the claiming system. 

- **/claimpvp**
  - This command will enable players to fight each other inside a claim. There is a 30 second delay between the command and actually changing the claim's status. All players who are inside the claim are warned, so no one is taken by surprise.
  - Uses the *griefprevention.claims* permission, which is given to all players by default

- **/eject [player]**
  - Got a bunch of players in a claim who are bothering you? Simply use this command and anyone who does not have some form of trust will be removed from the claim. In order to use this command, the player must either be the claim owner or be /trust ed to the claim.
  - To use it, simply stand in the claim you want to eject players from.
  - If a specific player is supplied, that player will be barred from entering that claim again for 1 hour.
  - This uses a new permission node, *griefprevention.eject*, which defaults to everyone
  - Want to make sure certain players aren't ejected from a claim? Give them *griefprevention.noeject*
  
- **/allowenter &lt;player&gt;**
  - This command will allow a player who was barred from entering a claim with /eject to enter it again. 
  - This command also uses the *griefprevention.eject* node.

- **/claimprotect**
  - Makes a claim protected from damage, even from owners/builders.
  
- **/removeoldclaims**
  - Can only be run from the console
  - Manually removes claims that should have expired, 25 at a time. Use this if the regular removal system can't keep up with the number of expired claims.

- **/adjustaccruedclaimblocks**
  - Used to adjust the number of claimblocks given from the game (as opposed to bonus claimblocks)
  - requres permission *griefprevention.adjustclaimblocks*

### Misc

[Download link!](https://github.com/10becja/MinecraftPlugins/raw/master/GriefPreventionPVP/GriefPrevention.jar)  

[GriefPreventionPVP repository](https://github.com/10becja/GriefPreventionPVP)

Found a bug or want to request a feature? Please let me know [here!](https://github.com/10becja/GriefPreventionPVP/issues)

Come play minecraft with us at [play.minecraft.dk!](minecraft.dk)

