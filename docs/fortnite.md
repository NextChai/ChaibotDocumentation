## Fortnite:
**All Fortnite related commands**. Any command in need of Chai Verification will be specified.
 
The Verification command will be listed first - just so it is easy to reference.
 
### **setverification**
**Setup a channel for Chai verification**. Any member that completes verification is agreeing to have some of their information shared to an API upon an authorized request. Any person with access to this private data is strictly monitored to maintain a safe environment. This command is toggleable.
 
**By default, a members nickname will be changed to their ign. You can disable this with: chaitogglenickchanges**
 
*Set the FN verification*
 
Requirements:
- Manage channels permission
 
How to use:
```
chaisetverification [channel:discord.TextChannel=None]
```
Useage Example
```
chaisetverification
 
chaisetverification #verification
```
 
### **togglenickchanges**
Toggle the default nickname changes that comes with Chai Verification.
 
*Enable/disable nickname changes*
 
Requirements:
- Manage channels permission
 
How to use:
```
chaitogglenickchanges
```
 
### **getstat**
**Get the Battle Royale stats of another member** or yourself. The member / user must be verified in order to perform this command.
 
*Get a verified members stats.*
 
How to use:
```
chaigetstat [member:discord.Member=None]
```
Usage Example:
```
chaigetstat
 
chaigetstat @Chai#1000
```
 
### **prcheck**
**"Prcheck" another member** or yourself. This command uses the [Fortnite Tracker API](https://fortnitetracker.com/site-api) to get accurate PR and Earnings. The member / user must be verified in order to perform this command.
 
*PR check's someone lol*
 
Prcheck yourself or another person.

How to use:
```
chaiprcheck Optional[subcommand] member[discord.Member=None]
```

Useage Example:
```
chaiprcheck
chaiprcheck @chai

chaiprcheck fast
chaiprcheck fast @chai
```

 
### **setitemshop**
**Set a custom channel for Item Shop Updates**. This is the same function as what's in the **chaisetup** command, but allows for channel customization (chaisetup does not allow for channel customization). This command is toggleable.
 
**The channel the command is used in will become the update channel.**
 
*Custom item shop updates*
 
Requirements:
- Manage channels permission
 
How to use:
```
chaisetitemshop
```
 
### **setnews**
**Same applies to setnews that applies to the setitemshop command** (as shown above). The only difference is it will setup a custom news channel instead of a custom item shop channel. This command is toggleable.
 
**The channel the command is used in will become the update channel.**
 
*Sets up a channel for custom news updates*
 
Requirements:
- Manage channels permission
 
How to use:
```
chaisetnews
```

### **verify**
Verify without having Fortnite Verification enabled through a reaction role. Your Dm's must be open in order for this command to work properly.

How to use:
```
chaiverify
```

Use Example:
```
chaiverify
```

### **unverify***
Don't want to be verified anymore? Get rid of it! 

How to use:
```
chaiunverify
```

Use Example:
```
chaiunverify
```