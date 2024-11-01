# OBS TrembleTalk!!!!!!!!!!

- Built using Python 3.11.9
- Ran on OBS Studio 30.2.3

<br/><br/><br/>

# How it works

- When PyAudio detects dB levels above a certain level, OBS TrembleTalk will start the playback of Media Source.
- When silence is detected for more than .30 seconds, it stops the playback of Media Source and resets the timestamp to 0.
- By default, Toggle Shake Effect is **OFF**. If you toggle Shake Effect to be ON, as the volume of your voice rises, so does the severity of the shake. The video will shake. Its great. 

<br/><br/><br/>

# Required Imports

```bash
pip install pyaudio
```
```bash
pip install numpy
```

<br/><br/><br/>

# How To Run OBS TrembleTalk in OBS Studio 30.2.3

### Add OBS TrembleTalk to OBS Scripts

![Select Tools](https://github.com/Duck1776/OBS-TrembleTalk/blob/main/img/image.png)
![Select Scripts](https://github.com/Duck1776/OBS-TrembleTalk/blob/main/img/image-1.png)
![Press the Plus Icon](https://github.com/Duck1776/OBS-TrembleTalk/blob/main/img/image-2.png)
![Open py file](https://github.com/Duck1776/OBS-TrembleTalk/blob/main/img/image-3.png)

<br/><br/>

### **Point OBS to your Python.exe folder location**

<br/>

![Go to Python Settings](https://github.com/Duck1776/OBS-TrembleTalk/blob/main/img/image-4.png)
![Brows to Python Path](https://github.com/Duck1776/OBS-TrembleTalk/blob/main/img/image-5.png)


<br/><br/>

### **On the main OBS interface, in Source, add a Media Source, and browse for your video**

<br/>

![Add Media Source](https://github.com/Duck1776/OBS-TrembleTalk/blob/main/img/image-6.png)

<br/><br/>

### **Whatever you name your Media Source, as it shows in the Sources area, enter that name into the Media Source field for the OBS TrembleTalk Script.**

You can set up to 4 Scenes in the Script to run only when the active Scene is active. Names must match.


> :warning: **Warning:** **THIS IS CASE SENSITIVE**

<br/>

![Fill in fields](https://github.com/Duck1776/OBS-TrembleTalk/blob/main/img/image-7.png)

<br/><br/>

**Refresh the Script - Script will run once it can compute audio** [^1]

![Refresh Python](https://github.com/Duck1776/OBS-TrembleTalk/blob/main/img/image-8.png)

<br/><br/>


[^1]: **Script will run once it can compute audio** - OBS TrembleTalk uses [PyAudio](https://pypi.org/project/PyAudio/) to detect input audio streams and the dB of that audio. No configuration needed.
