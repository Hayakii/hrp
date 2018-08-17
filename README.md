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

## CLIENTS SIDE FUNCTIONS
### HAY.serverPrint(message)
Print text in the server's console
- *char* **@message** : Message to print
```lua
HAY.serverPrint(message)
```

## SERVER SIDE FUNCTIONS
### HAY.withdrawMoney(source, value, callback)
Withdraw money from a player's bank account.
- *int* **@source** : Server ID of the player
- *int* **@value** : Amount to withdraw
- *func* **@function** : Callback
 - *bool* **@state** : return true of false
 - *string* **@message** : return a message
```lua
HAY.withdrawMoney(source, value, function(state, message)
  -- Do stuff in callback
end)
```

### HAY.depositMoney(player, value, callback)
Deposit money to bank account.
- *int* **@source** : Server ID of the player
- *int* **@value** : Return amount of money
- *func* **@function** : Callback
 - *bool* **@state** : return true of false
 - *string* **@message** : return a message
```lua
HAY.depositMoney(source, value, function(state, message)
  -- Do stuff in callback
end)
```

### HAY.getPlayerMoney(player, callback)
Return amount of money of a player.
- *int* **@source** : Server ID of the player
- *func* **@function** : Callback
 - *int* **@value** : Return amount of money
```lua
HAY.getPlayerMoney(source, function(value)
  -- Do stuff in callback
end)
```

### HAY.createCreditCard(player, callback)
Create a credit card and return if it successfuly created it.
- *int* **@source** : Server ID of the player
- *func* **@function** : Callback
 - *int* **@value** : Return true of false
```lua
HAY.createCreditCard(source, function(result)
  -- Do stuff in callback
end)
```

### HAY.hasCreditCard(player, callback)
Return if the player has a credit card.
- *int* **@source** : Server ID of the player
- *func* **@function** : Callback
 - *bool* **@result** : Return true of false
```lua
HAY.hasCreditCard(source, function(result)
  -- Do stuff in callback
end)
```

### HAY.createBankAccount(player, callback)
Create a bank account and return if it successfuly created it.
- *int* **@source** : Server ID of the player
- *func* **@function** : Callback
 - *int* **@value** : Return true of false
```lua
HAY.createBankAccount(source, function(result)
  -- Do stuff in callback
end)
```

### HAY.hasBankAccount(player, callback)
Return if the player has a bank account.
- *int* **@source** : Server ID of the player
- *func* **@function** : Callback
 - *bool* **@result** : Return true of false
```lua
HAY.hasBankAccount(source, function(result)
  -- Do stuff in callback
end)
```

### HAY.print(message)
Print text in the server's consol adding `[HRP]` prefix.
- *char* **@message** : Text to print
```lua
HAY.print(message)
```

### HAY.writeLog(message)
Write text in log file.
- *char* **@message** : Text to write
```lua
HAY.writeLog(message)
```

### HAY.player.steamid(player)
Return steamid or license of a player.
```lua
HAY.writeLog(message)
```
