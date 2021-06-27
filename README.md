# Davinci Resolve Media Converter.

***davincimc*** is a Linux script 🐧, it help you to convert Media and import it into davinci resolve. (for windows of Mac [click hare](#windows-and-mac))!

## Dependency 🇲🇦.
You have to install **FFMPEG**:

- Debian/Ubuntu(PopOs,  LinuxMint, ElementaryOs, MxLinux...)
```terminal
sudo apt update
sudo apt install ffmpeg
```
- Fedora
```terminal
sudo dnf -y install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm
sudo dnf -y install https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm

sudo dnf update
sudo dnf install -y ffmpeg
```
- OpenSUSE
```terminal
sudo zypper install opi
opi codecs
```
## Instalation
Clone this reposotory or Download the latest [release version](https://github.com/zakaria-chahboun/davinci-resolve-media-converter/releases/tag/1.0).
```terminal
sudo ./install
```

## How to use ?
```
davincimc INPUT.mp4 --MODE
```

### We have two modes:
- *--video*: to convert any video format to (.MOV)
- *--audio*: to extract any media format to (.wav)


### Example:
```
davincimc ./mymedia/video.mp4 --video
```
```
davincimc ./mymedia/podcast.mp4 --audio
```
```
davincimc ./mymedia/podcast2.mp3 --audio
```

> **The new output Media File has the same name as your file, in the same directory with (the new) extension ✌.**

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
## Windows and Mac
**if you are using Windows or Mac you have to do this manually!**

**download FFMPEG for any os .. <a href='https://www.ffmpeg.org/download.html'> here </a>**

```
ffmpeg -i INPUT.mp4 -c:v dnxhd -profile:v dnxhr_hq -pix_fmt yuv422p -c:a pcm_s16le OUTPUT.mov

ffmpeg -i INPUT.mp4 -c:a pcm_s16le OUTPUT.wav
```

thanks to <a href="https://linuxgamecast.com/2019/08/davinci-on-linux-import-mp4-mp3/">linuxgamecast</a>
