
# Welcome to Chaibot Documentation

Chaibot's commands with how-two's and examples. [https://top.gg/bot/728115804826239017](https://top.gg/bot/728115804826239017).

## How to use:
Below are all commands for Chaibot, sorted in **custom categories (cogs) for each set of commands**. Using the navigation on the left is a big help, I recommend making use of it.

Any **command in need of special permissions will be specified**. If not specification is given, the command requires no perms.

Any command that is toggleable (used once to turn on and once again to turn off) will be specified. 

The "How to Use" section.
- The how to use section will show you the name for the parameter folllowed by its type. For example: **[name: type]**

- Here's some examples of things you will see:
    ```
    discord.Member: a server membe
    discord.Role:  a server role
    str: a "string" (aka a text)
    int:  a number
    ```
## Main Commands:
Command sections are seperated in cogs. You can do **chaihelp CogName** for more info on a cog. All commands are shown with the **chai** prefix, easily change out this prefix and use your own one.

## Commands Cog:
### **aes**
Display the current **AES Key and Version** from Fortnite Battle Royale.

How to use:
```
chaiaes
```

### **aesdump**
Display any **decrypted AES data** from Fortnite Battle Royale.

How to use:
```
chaiaesdump
```

### **creatorsearch**
Search any **Fortnite Creator Code** and recieve some useful information.

How to use:
```
chaicreatorsearch [creatorCode:str]
```

Useage Example:
```
chaicreatorsearch Ninja
```

### **getrlstat**
Search any Steam Account and recieve **Rocket League rank** information. This command only applies to Steam, it does not support Epic Games, Xbox, PSN, or Switch. Psyonix and Epic have not released an official endpoint to get Rocket League stats yet, so we're very limited.

You can input a Steam ID or a Steam name.

How to use:
```
chaigetrlstat [steamAccount:str]
```

Useage Example:
```
chaigetrlstat chaiski

chaigetrlstat 123456321334
```

### **guilds**
Recieve a **number of how many servers Chai is currently in.**

How to use:
```
chaiguilds
```

### **invitechai***
Recieve an **invite for Chai**, allowing members of your server to get Chai in their servers if they desire.

How to use:
```
chaiinvitechai
```
## Setup:
**Setup your server for Chai updates**. This command walks you through which updates you want.

Requirements:
- Manage Channels Permission

How to use:
```
chaisetup
```

## API Cog:
Discord API exclusive things. Use commands inside of this cog to **navigate the discordpy library**.

Code idea from [R.Danny](https://github.com/Rapptz/RoboDanny), **none of the code in R.Danny is used in Chai**.

### **rtfm**
Gives you a documentation link for the [discord.py](https://discordpy.readthedocs.io/en/latest/) library. Events, objects, and functions are all supported through a fuzzy algorithm.

rtfm jp:
- Gives you a documentation link for a discord.py entity (Japanese).

rtfm py-jp 
- Gives you a documentation link for a Python entity (Japanese).

How to use:
```
chairtfm [query:str]

chairtfm jp [query:str]

chairtfm py-jp [query:str]
```

Useage Example:
```
chairtfm discord.Message

chairtfm jp discord.Message

chairtfm py-jp str
```

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
**Get the Battle Royale stats of another member** or yourself. The member / user must be verified in order to peform this command.

*Get a verified members stats.*

How to use:
```
chaigetstat [member:discord.Member=None]
```
Useage Example:
```
chaigetstat

chaigetstat @Chai#1000
```

### **prcheck**
**"Prcheck" another member** or yourself. This command uses the [Fortnite Tracker API](https://fortnitetracker.com/site-api) to get accurate PR and Earnings. The member / user must be verified in order to peform this command.

*PR check's someone lol*

How to use:
```
chaiprcheck [member:discord.Member=None]
```

Useage Example:
```
chaiprcheck

chaiprcheck @Chai#1000
```

### **setitemshop**
**Set a custom channel for Itemshop Updates**. This is the same function as what's in the **chaisetup** command, but allows for channel customization (chaisetup does not allow for channel customization). This command is toggleable.

**The channel the command is used in will become the update channel.**

*Custom itemshop updates*

Requirements:
- Manage channels permission

How to use:
```
chaisetitemshop
```

### **setnews**
**Same applies to setnews that applies to the setitemshop command** (as shown above). The only difference is it will setup a custom news channel instead of a custom itemshop channel. This command is toggleable.
 
**The channel the command is used in will become the update channel.**

*Sets up a channel for custom news updates*

Requirements:
- Manage channels permission

How to use:
```
chaisetnews
```

## Fun
All fun commands of Chai. Any command inside of this cog is available to any member that can send messages.

*Fun commands*

### **commands_used**
Get a **number of commands used in the current session.**

How to use:
```
chaicommands_used
```

### **hello**
Heya! Similar to the ping command, **have Chai say hello back to you**.

How to use:
```
chaihello
```

### **member_info**
**Get some information on another member** in your server. All information displayed from this command is public, and does not display any inforamtion used in Chai Verification.

How to use:
```
chaimember_info [member:discord.Member=None]
```
Useage Example:
```
chaimember_info

chaimember_info @Chai#1000
```

### **ping**
**Ping Chai and get a latency number** back. Mainly used by the dev, this command can be useful to determine if Chai is lagging.

How to use:
```
chaiping
```

### **uptime**
Get the **current uptime** for Chai.

How to use:
```
chaiuptime
```

## Logs
Handling the logging system.

Chai's logging system is broken down into a command group, meaning you can control everything with one command. We're going to run down a line to get your logging sytem up and running.

### **logs**
This command is the first command to get your log system working. **chailogs will enable your server for logs, it will not enable any logs**. Those can be toggled with the command group commands (as shown down below). All commands in this cog require the manage channels permission.

Any subcommand shown without a *How to use* section has no parameters, you just use the commmand by itself.

**The channel this command is done is will be your logging channel (you can change this later).**

*Handle the logging sytem*

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
Useage Example:
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

## Moderation:
All moderation commands for Chai. Any command in this cog that needs special permissions will be listed.

### **ban**
**Ban a member** from your discord. 

Requirements:
- Ban members permission

How to use:
```
chaiban [member:discord.Member] [reason:str=None]
```
Useage Example
```
chaiban @Chai#1000

chaiban @Chai#1000 using memes in general :kek:
```

### **kick**
**Kick a member** from your discord. 

Requirements:
- Kick members permission

How to use:
```
chaikick [member:discord.Member] [reason:str=None]
```
Useage Example
```
chaikick @Chai#1000

chaikick @Chai#1000 using memes in general :kek:
```

### **prefix**
**Change Chai's default prefix** ("chai"), to any prefix you want.

Requirements:
- Manage channels permission

How to use:
```
chaiprefix [prefix:str]
```

Useage Example:
```
chaiprefix !
```

### **purge**
**Purge a channel** a specified amount of messages.

Requirements:
- Manage channels permission

How to use:
```
chaipurge [limit:int]
```

Useage Example:
```
chaipurge 100
```

### **invite**
**Crate an instant invite** to your server. This invite is set not to expire, so be sure to keep that in mind when using it.

Requirements:
- Manage channels permission

How to use:
```
chaiinvite
```



## Warning System:
Part of the Moderation cog, diserves its own section due to its type. All commands in this section require the manage channels permission

### **warn**
**Warn a member** for something they've done incorrect. This will keep a log of their warnings and alert them that they've been warned.

How to use:
```
chaiwarn [member:discord.Member] [reason:str=None]
```

Useage Example:
```
chaiwarn @Chai#1000 saying no no words

chaiwarn @Chai#1000
```

### **warnings**
**Check a members past warnings.**

How to use:
```
chaiwarnings [member:discord.Member]
```

Useage Example:
```
chaiwarnings @Chai#1000
```

### **clearwarnings**
Clear a members warnings.

How to use:
```
chaiclearwarnings [member:discord.Member]
```

Useage Example:
```
chaiclearwarnings @Chai#1000
```

## Music
The music handing system for Chai.

The music cog for Chai. Chai is not being hosted on a VPS rn, it's locally hosted. This means the PC its being hosted on
isn't great. Because of this, music may be laggy / some bugs.

Nevertheless, Chai has music support for Spotify, YouTube, Twitch, SoundCloud, and many more.

### **connect**
Have Chai connect to your channel.

How to use:
```
chaiconnect
```

### **play**
Have Chai **play a song**. Chai has support for Spotify, YouTube, Twitch, SoundCloud, and many more. You can paste the link for your song as your song param to play it.

How to use:
```
chaiplay [song:str]
```
Useage Example:
```
chaiplay Sicko Mode
```

### **skip**
Have Chai skip the current song onto the next one in the queue.

How to use:
```
chaiskip
```

### **pause**
Pause the current song

How to use:
```
chaipause
```

### **resume**
Resume the paused music.

How to use:
```
chairesume
```

### **queue**
Add a song to your queue. This is an alias for the **play** command, which will also add songs to your queue. 

If this command is used without the song param, it will **display the current queue.**

How to use:
```
chaiqueue [song:str=None]
```
Useage Example:
```
chaiqueue Sicko Mode

chaiqueue
```

### **shuffle**
Shuffle your current queue.

How to use:
```
chaishuffle
```

### **volume**
Change Chai's volume. The volume can range anywhere from 0 to 1000.

How to use:
```
chaivolume [volume:int]
```
Useage Example
```
chaivolume 1000
```

### **stop**
Stop the current song and leave your call.

How to use:
```
chaistop
```

### **now_playing**
Get the some information on the current song.

How to use:
```
chainow_playing
```

### **musicinfo**
View Chai music server info. Get some information on Chai's music server.

How to use:
```
chaimusicinfo
```

## Reaction Roles:
Chai reaction roles is something I plan on focusing a lot on in the next couple of weeks. I'm going to lay it out as simple as possible for you to set them up. 

Reaction roles have a max of 5 emojis total, assigning to 5 individual roles.

**The commands in this list must be done in ascending order**

All commands in this Cog require the manage channels permission.

### **reactionrole**
Sets up the initial embed. This is what we're going to add our emoji's to and assign roles. Each param must be in "".

**How to use:**
```
chaireactionrole [title:str] [description:str] [name:str] [value:str]
```
Title: The Embed title.

Description: The Embed Description.

Name: The Embed field's name.

Value: The Embed field's value.

**Useage Example:**
```
chaireactionrole "this is a title" "this is a description" "this is a name" "this is a value -

that can be mutiple lines because it's in quotes."
```

### **reactionadd**
Let's add an emoji to our embed and assign it to a role. 

How to use:
```
chaireactionadd [emoji:discord.Emoji] [role:discord.Role]
```

Useage Example:
```
chaireactionadd 😋 @Fortnite

chaireactionadd :blush: @Rocket League
```

### **reactionroleremove**
Disable the use of the reactionrole embed. This is optional - you can always just delete the message.

How to use:
```
chaireactionroleremove
```