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