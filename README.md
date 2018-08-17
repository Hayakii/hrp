# Havana Framework
## Getting started
1. Place `hay_framework` in the ressource folder of your fivem server.
2. Add `start hay_framework` in your server.cfg file.
3. To use the framework you need to add both of this lines into your `__resource.lua` resource file.
```lua
server_script ''
client_script ''
```
4. Your done ! You can now use the framework :)

## Clients functions
#### HAY.serverPrint(message)
Print text in the server's console
```lua
HAY.serverPrint(message)
```
