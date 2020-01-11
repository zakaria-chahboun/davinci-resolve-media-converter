# Davinci Resolve Media Converter For LINUX!

***davincimc*** is a script, it help you to convert Media and imported into davinci resolve (15)!

Dependency: you have to install **FFMPEG**.

### How to use
```
davincimc INPUT.mp4 --MODE
```

### We have two modes:
- *--video*: to convert any video format to special (.MOV)
- *--audio*: to extract any media format to special (.wav)


### Example:
```
davincimc ./mymedia/podcast.mp4 --video
```

> **The new output Media File has the same name as your file, in the same directory with (new) extension.**

### Help
You can get help by using:
```
davincimc --help
```
or
```
davincimc -h
```

<img src="https://i.udemycdn.com/course/750x422/2373482_a71b_3.jpg" alt="davinci resolve logo"/>

--------------

**if you are using Windows or Mac you have to do this manually!**

**download FFMPEG for any os .. <a href='https://www.ffmpeg.org/download.html'> here </a>**

```
ffmpeg -i INPUT.mp4 -c:v dnxhd -profile:v dnxhr_hq -pix_fmt yuv422p -c:a pcm_s16le OUTPUT.mov

ffmpeg -i INPUT.mp4 -c:a pcm_s16le OUTPUT.wav
```

thanks to <a href="https://linuxgamecast.com/2019/08/davinci-on-linux-import-mp4-mp3/">linuxgamecast</a>
