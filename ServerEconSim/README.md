
#ServerEconSim

This plugin attempts to have the server emulate a player by allowing it to make "requests" that players can fulfill.

To fulfill a request, a player simply needs to go to a Request Board, and right click on it with enough of that item in their inventory.

To make a Request Board, place a sign and enter `{RB}` on the second line, and the request slot on the third line. For example, if you have the plugin set up to pick 5 requests, and you want to set up a sign to show the 4th request, your sign would look like:
```
|             |
|     {RB}    |
|       4     |
|             |
```

Signs automatically update whenever new requests are generated. Breaking a sign will remove it from the signs.yml file.

### Dependencies:
- [Vault](http://dev.bukkit.org/bukkit-plugins/vault/)
- Some sort of economy plugin

### Config.yml:
```
Value fluxuations:
- 0
- 10
- 25
- 50
- 100
- 500
Seconds until requests are refreshed: 86400
Number of requests: 5
Broadcast new requests: true
```

Most are fairly self explanatory. The `Value fluxuations` list is used to fluxuate the price of a request, based on how valuable that request is (more on this later). The value will flux between -amount and +amount. For instance, if you have a request that has a base price of 25, and a value of 1, the price could fluxuate anywhere between 15 and 35.

### request.yml
This is an example of a request you might see in this file
```
  '1':
    item: '{"==":"org.bukkit.inventory.ItemStack","damage":3,"type":"STONE"}'
    displayName: Diorite
    amount: 100
    price: 25
    value: 1
    timesBought: 0
    limit: 1
```
Really the only values you should edit in this are the `displayName`, `amount`, `price`, `limit`, and `value`, if you want to make manual changes. Manually editing the `item` could cause problems if you don't know what you're doing. `timesBought` is a counter to keep track of how many times that particular request has been used.


### Commands:
- **/setrequest &lt;amount&gt; &lt;price&gt; &lt;value&gt; &lt;limit&gr; (display name)**
  - Sets up a request for the server.
  - To use this, first hold the item you want to make a request of, the run the command
  - The `<value>` is used for determining how greatly the price can fluxuate
  - If you don't provide a display name, the plugin will use the default name of the item you are holding. However, because of how bukkit works, this might not be the correct name. For example, if you make a request for Diorite, but don't provide a display name, it will be stored as STONE. 
  - `<limit>` is the number of times this request can be fulfilled per player in the configured time span. 

- **/viewrequests**
  - Shows the current requests
  - Green requests have not been completed by you.
  - Red indicates that you've already done that request

- **/listrequests (filter) [page]**
  - Displays all available requests, 10 at a time
  - Use `[page]` to show specific pages
  - If you want to only see specific requests, say all requests involving the word "leaves", use the `(filter)`

- **/requestdetails &lt;id&gt;**
  - Gives all details related to that request

- **/editrequest &lt;id&gt; &lt;amount&gt; &lt;price&gt; &lt;value&gt; &lt;limit&gr; (display name)**
  - This functions very similar to **/setrequest**
  - It allows you to update request data ingame, rather than needing to edit the backend file.

- **/reloadrequests**
  - Reloads the plugins.

### Permissions
- *ses.setrequest* : allows use of **/setrequest** and **/editrequest**
- *ses.viewrequests* : allows use of **/viewrequests**
- *ses.listrequests* : allows use of **/listrequests**
- *ses.requestdetails* : allows use of **/requestdetails**
- *ses.makesign* : allows you to create Request Boards
- *ses.breaksign* : allows you to break Request Boards
- *ses.admin* : allows for **/reloadrequests**

[Download link!](https://github.com/10becja/MinecraftPlugins/raw/master/ServerEconSim/ServerEconSim.jar)  

[ServerEconSim repository](https://github.com/10becja/ServerEconSim)

Found a bug or want to request a feature? Please let me know [here!](https://github.com/10becja/ServerEconSim/issues)
