
#MinecraftClassifieds

Some brief info about plugin

### Dependencies:
- [Vault](http://dev.bukkit.org/bukkit-plugins/vault/)
- Some sort of economy plugin
- [Essentials](http://dev.bukkit.org/bukkit-plugins/essentials/)

### Config.yml:
```
TBD
```


### Commands:
- **/mccrequest**
  - This command will initialize a wizard that will prompt the user through selecting the items they want
  - To exit the wizard at any time type 'Quit' into chat.
  - When you confirm the request, it will deduct the amount of the request from your balance.
  - If the request is cancelled before it is fulfilled, you will be refunded your money

- **/mcclist (mine|player name) [page]**
  - using just the command will list all active requests, ordered by create date.
  - using '/mcclist mine' will display all of your requests, including ones that are ready for collection.
  - use the `[page]` to view multiple pages of requests

- **/mccfulfill &lt;id&gt;**
  - Once you have the items for a specific request, use this command to fulfill it. The items will be removed from your inventory and you will be credited the money.

- **/mccget &lt;id&gt;**
  - Once a request has been fulfilled, you can get the items by using this command. Please note, this id is the id from `/mcclist mine`, not the list of active requests.

- **/mcccancel (player) &lt;id&gt;**
  - Allows you to cancel one of your requests, or someone else's
  - Again uses the `/mcclist mine` or `/mcclist playerName`

- **/mccreload**
  - Reloads the config.

### Permissions
- tbd

[Download link!](https://github.com/10becja/MinecraftPlugins/raw/master/MinecraftClassifieds/MinecraftClassifieds.jar)  

[MinecraftClassifieds repository](https://github.com/10becja/MinecraftClassifieds)

Found a bug or want to request a feature? Please let me know [here!](https://github.com/10becja/MinecraftClassifieds/issues)
