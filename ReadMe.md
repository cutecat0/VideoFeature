<h1>Video Feature</h1>

This part mainly records video feature
<img width="4191" alt="video dessert" src="https://user-images.githubusercontent.com/37787934/155257003-e5ca18c6-b231-4424-b3e4-6ab458b60f22.png">

<h2>What's M3U8?</h2>
e.g<br>
"m3u8": "#EXTM3U\n#EXT-X-TARGETDURATION:10\n#EXTINF:9,\nhttp://xxx.ts?start=0&end=xxxx&contentlength=xxxx&........=0\n#EXTINF:9,\nhttp:xxxx0.ts?start=xxxx&end=xxx&contentlength=xxxx&......=0\n
...#EXTINF:9,\nhttp:xxx.ts?start=xxxx&end=xxx&contentlength=xxx&.....=0\n#EXTINF:9....<br>
In this m3u8, it owns different xxx.ts file with end and start tag.<br>
When user watching video, it can be displayed from one ts to another ts file without load whole video file, 
which is all m3u8 file.<br>
**So, what's the advantage user this way?**<br>
1. It makes the video more smooth with less stuck.<br>
2. If there's ABS, it helps seerver to make more effective bitrate.<br>
3. Under worse network, it can be much useful to support the video can always display without stop(stuck too long).<br>

`<h3>Video Display Process</h3>
1. Server collect bitrate video to slice machine<br>
2. Slice machine create index file for video and cut it into N numbers of ts file<br>
3. Passing above 2 files (index file & ts file) on http server<br>
4. Website or Client App searching for ts file on http server according to index file, then display N numbers
of ts file, and that will be okay, which means, display done.<br>
   
So, as we all know that, index file is so much important.<br>
And, guess what! Here, **the index file is M3U8 file!!!**<br>
`
<h1> some useful site of video feature</h1>
1. https://mp.weixin.qq.com/s/Psgd7Jx7Yf38ULuZncZvcw<br>
2. https://mp.weixin.qq.com/s/Oktehrz7x0OIaDvXlzMenw<br>
3. https://mp.weixin.qq.com/s/FC4_QXrX3UmqYl6Mp82okA<br>
4. https://mp.weixin.qq.com/s/C1OfqDPkGkU6wrRNimCeGw<br>
5. https://mp.weixin.qq.com/s/YGPSyHeipdmJ0trCQBBwVA<br>
6. https://mp.weixin.qq.com/s/CoOf_SYMWIgb4gCyAFHy9g<br>

<h1>What's video bitrate?</h1>
reference: https://restream.io/blog/what-is-video-bitrate/<br>
Video bitrate defines video data transferred at any given time.<br>
Bitrate is measured in bits per second, which is referred to as “bps.”<br>
![img.png](img.png)<br>
to be updated....<br>

https://filmora.wondershare.com/video-editing-tips/what-is-video-bitrate.html
1. file size<br>
2. codec<br>
3. delivery cost<br>
4. CBR / VBR:  constant bit rate  / variable bit rate <br>
5. audio : same logic<br>
6. calculate file size<br>

#TBD
###The difference between video bitrate. bitrate streaming?

<h1>WebRTC</h1>
https://mp.weixin.qq.com/s/YGPSyHeipdmJ0trCQBBwVA<br>
RTP\RTMP\

# video decode and some other features

![image](https://user-images.githubusercontent.com/37787934/161378375-f1ed56cb-5622-42fe-adc7-e45f0f12de6a.png)


# Some Useful Site
1. https://www.brid.tv/future-of-video-technology/
2. https://www2.deloitte.com/content/dam/insights/us/articles/4479_Digital-media-trends/4479_Digital_media%20trends_Exec%20Sum_vFINAL.pdf