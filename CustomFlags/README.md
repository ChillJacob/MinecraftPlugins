
#CustomFlags

Simple plugin that adds additional flags to worldguard regions:

Sample `flags.yml`

```
# Flags available
# 
# nomobdamage: Prevent taking damage from mobs
# nohunger: Prevent losing hunger
# noportals: Prevent nether portals from being generated
# noteleport: Prevent any form of teleporting into or out of an area. Add customflags.bypass.noteleport to bypass
MyWorld:
  spawn:
  - nohunger
  - noportals
MySafeWorld:
  __global__:
  - nomobdamage
```


### Commands:
- **/loadflags**
  - Reloads the flags and config files.
   
### Permissions
- *customflags.bypass.noteleport* : allows teleporting in/out of regions with the `noteleport` flag
- *customflags.admin* : allows use of **/loadflags**

[Download link!](https://github.com/10becja/MinecraftPlugins/raw/master/CustomFlags/CustomFlags.jar)  

[CoinExchange repository](https://github.com/10becja/CustomFlags)

Found a bug or want to request a feature? Please let me know [here!](https://github.com/10becja/CustomFlags/issues)
