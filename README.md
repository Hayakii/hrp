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
## How it works ?
In this section, you can learn how the framework works and find out what each file is about.

## Clients functions
### HAY.serverPrint(message)
Print text in the server's console
> char @message : Message to print
```lua
HAY.serverPrint(message)
```

## Server functions
### HAY.withdrawMoney(source, value, callback)
Withdraw money from the player's bank account.
*int* **@source** : Server ID of the player
*int* **@value** : Amount to withdraw
*func* **@function** : Callback
  *bool* **@state** : return true of false
  *string* **@message** : return a message
```lua
HAY.withdrawMoney(source, value, function(state, message)
  -- Do stuff in callback
end)
```
