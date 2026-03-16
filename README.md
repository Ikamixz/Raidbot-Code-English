# RaidBot English

**General Information**

RaidBot is a Discord bot developed in Python using the discord.py library (https://github.com/Rapptz/discord.py). Its purpose is to automate administration and testing tasks on Discord servers, offering commands that allow for everything from basic management (latency, roles, channels) to advanced functions such as channel cleanup, resetting, and sending bulk messages.

This project is intended for **educational and experimental** purposes, showing how to build custom commands, manage permissions, and work with events in Discord.

---

**Requirements**

- Python 3.9 or higher
- Windows

Install them with:
```Setup.Py
```
## RaidBot Commands Explanation

RaidBot includes a series of commands designed to interact with Discord servers. Each one serves a specific function:

- **`$hlp`**  
  Displays a help panel with the complete list of available commands and their descriptions.

- **`$ping`**  
  Returns the bot's latency in milliseconds, useful for checking if it is responding correctly.

- **`$spam`**  
  It sends a large number of repeated messages across all text channels on the server.

- **`$raid`**  
  Create multiple text channels with a base name..

- **`$nuke`**  
  Remove all channels from the server immediately.

- **`$cn`**
  Change the server name to a new one defined in the code.

- **`$cr (cantity)`**  
  Create a specified number of roles on the server, with sequential names.

- **`$ci`** 
Change the server icon to an image located in the same folder as the bot.

- **`$ret`** 
Delete all existing channels and then create new channels with mass spam in each.

- **`$bn`** 
Ban all members of the server, except the command author, the owner, and the bot itself.

- **`$db (USER ID)`** 
Unban a user using their ID.

- **`$sv`** 
It displays a list of servers where the bot is located.

- **`$dr`** 
Remove all server roles, except protected ones (such as the default role, the owner, and the bot).

- **`$ks (Server ID)`** 
Schedule the automatic execution of several commands when the bot joins a specific server.

- **`$vs (Server ID)`** 
Execute a set of raid commands on a remote server, only if the bot is present.

- **`$da (User ID) (Server ID)`** 
Create a role with administrator privileges and assign it to a specific user on the specified server.

- **`$md`** 
Sends direct messages (DMs) to all server members with a predefined embed code.

- **`$cleanbot (bot ID)`** 
Deletes messages sent by a specific bot in all server text channels.
- **`$cleanbot (bot ID)`** 
Deletes messages sent by a specific bot in all text channels on the server.

- **`$cleanraid (prefix)`** 
Deletes all channels whose name begins with a given prefix, useful for cleaning up channels created in raids.

- **`$resetchannel`** 
Deletes the current channel and recreates it empty, keeping the same name and category.

- **`$clear`** 
Deletes all messages in the current channel.

---

RaidBot not only includes classic administration and raid commands.
Thanks to functions like `$ks` and `$vs`, the bot can **automatically trigger various commands upon entering a server** or **execute them remotely** without direct intervention.

This demonstrates how a bot can coordinate multiple actions simultaneously and leverage Python's concurrency (`asyncio`) to execute hundreds of tasks at the same time without crashing.
---

**Important Note**:
These commands are powerful and directly modify the server structure. It is recommended to use them only in test environments or for educational purposes, as they can drastically alter a live server.

Discord Server : https://discord.gg/3NwMRyScs4
