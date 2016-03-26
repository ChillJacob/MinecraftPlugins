
#CoinExchange

This is a very simple plugin that allows you to have a secondary economy (or primary if you'd like!) to reward players for things such as voting.

After you install the plugin and run your server for the first time, you can set up various commands to be purchased in the `commands.yml` inside `plugin/CoinExchange`.

Please pay attention to the structure of that file. By default, it comes with 1 item set up already, which allows players to exchange 10 coins for $1000, if you are using essentials economy. The plugin allows you to have multiple pages, and each page allows for up to 18 items. If you wish to add a new page, simply create a new section under `pages:` like such (remember to use proper yaml spacing):

```
page-x:
   slot-1:
     command: 
     price:
     displayItem:
     displayText:
```
     
The fields are fairly self explanatory. `Command` is the command that will be run, `price` is how many coins this command costs, `displayItem` is the item code of the item that will show in the GUI, and `displayText` is what will be displayed to the player when they hover over the item.

Because of how this plugin is set up, there are no dependencies. You can put any command you wish in the command, for any plugin you have running on your server. 

There is a section up at the top of the `commands.yml` file that will tell you what tokens are available to use. Right now, only `{player}` is supported, which will be set to the player who selected the command. 

Right now, the `config.yml` file has nothing of importance in it.


### Commands:
- **/addcoins <player> <amount>**
  - Adds coins to the player.

- **/removecoins <player> <amount>**
  - Remove coins from a player.

- **/viewcoins (player)**
  - Allows you to see how many coins you have. You can also use it to view other players coins.

- **/reloadcoins**
  - Reloads the commands and player storage files, along with the config.
   
### Permissions
- *coinexchange.addcoins* : allows use of **/addcoins**
- *coinexchange.removecoins* : allows for **/removecoins**
- *coinexchange.viewcoins* : allows you to use **/viewcoins** on yourself
  - *coinexchange.viewcoins.others* : use **/viewcoins** on other players
- *coinexchange.admin* : allows for **/reloadcoins**

[Download link!](https://github.com/10becja/MinecraftPlugins/raw/master/CoinExchange/CoinExchange.jar)  

[CoinExchange repository](https://github.com/10becja/CoinExchange)

Found a bug or want to request a feature? Please let me know [here!](https://github.com/10becja/CoinExchange/issues)
