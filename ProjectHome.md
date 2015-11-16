When I start to build a media play on TI's DaVinci platform, I found that I have to support divx, mkv, ... etc. I did and do think that I would need a framework to make everything simple.

I tried gstreamer, mplayer, and VLC.

I do think each of them is very great. But
1. mplayer has a very awful directory structure, so hard to read the code.
2. VLC, interface is combined in libvlc, that makes it a little fat.
3. gstreamer, I don't know why I should manager pipe each level.

What I need is one framework, which will focus on module management, such as demux, decode. Things like decode h.264 to use x264 or ffmpeg plugins is just left for a configure utility.

Hence birth the ezmedia.