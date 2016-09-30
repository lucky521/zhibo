
本地音视频设备
```
ffmpeg -f avfoundation -list_devices true -i ""
```

抓取Mac内置摄像头和内置麦克风数据流推送到RTMP
```
ffmpeg -f avfoundation -framerate 30  -i "0:0" -vcodec libx264  -acodec libfaac -f flv rtmp://172.16.33.133/hls/mystream
```

抓取本地文件推送到RTMP
```
ffmpeg -re -i SampleVideo.mp4  -vcodec libx264  -acodec libfaac -strict -2 -f  flv  rtmp://172.16.33.133/hls/mystream
```
