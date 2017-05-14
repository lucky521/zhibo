# zhibo 直播
Real Time Stream Practice

## Architecture

Stream Flow:  Anchor client --> RTMP Server  --> Audience Client


## RTMP
nginx-rtmp-module helps to build a RTMP service on [Nginx](./nginx/nginx.conf).

## HLS 
Here I use HLS Web Player Clappr to play HLS steam in web brower.

## FFmpeg
I use [FFmpeg](./ffmpeg/README.md) to generate video source stream at Anchor side. Then sent them to RTMP Server.
