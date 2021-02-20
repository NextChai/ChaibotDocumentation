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