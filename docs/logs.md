## Logs
Handling the logging system.
 
Chai's logging system is broken down into a command group, meaning you can control everything with one command. We're going to run down a line to get your logging system up and running.
 
### **logs**
This command is the first command to get your log system working. **chailogs will enable your server for logs, it will not enable any logs**. Those can be toggled with the command group commands (as shown down below). All commands in this cog require the manage channels permission.
 
Any subcommand shown without a *How to use* section has no parameters, you just use the command by itself.
 
**The channel this command is done is will be your logging channel (you can change this later).**
 
*Handle the logging system*
 
How to use:
```
chailogs
```
 
**Subcommands:**
 
**logs all**
 
Enable all of Chai's logging features for your server.
 
**logs channel***
 
Change the logging channel. Any channel you put in the command will be your new logging channel, and your old one will be invalidated.
 
How to use:
```
chailogs channel [newchannel:discord.TextChannel]
```
Usage Example:
```
chailogs channel #general
```
 
**logs channel_updates**
 
Get channel logging updates.
 
**logs guild**
 
Get guild logging updates.
 
**logs member**
 
Get member logging updates.
 
**logs messaage**
 
Get messaage logging updates. 
(I just realized this is spelt incorrectly, the command is spelt incorrectly (it only works as the incorrect spelling)- it is correct in the documentation and will work if you copy paste it)

