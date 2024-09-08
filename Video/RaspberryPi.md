# USB camera
Raspberry Pi / DietPi / NanoPi

## Video
### installation
```
sudo apt update
sudo apt install ffmpeg
```

### Recording
#### UltraFast
Best performance (low dropped frames) - 1h of recording create ~3GB file.
```
ffmpeg -f v4l2 -framerate 10 -video_size 800x600 -i /dev/video0 -c:v libx264 -preset ultrafast -t 1:00:00 output.mp4
```

#### FHD + jpg(every 4s)
```
sudo ffmpeg -f v4l2 -framerate 5 -video_size 1920x1080 -i /dev/video1 \
-c:v libx264 -preset ultrafast -t 1:00:00 -map 0:v \
-vf fps=5 output.mp4 -map 0:v -vf fps=1/4 output_image_%04d.png

```

## Take a picture/jpg
### Installation
```
sudo apt update
sudo apt install fswebcam
```

Preview of picture in ssh consolr
```
sudo apt-get install catimg
```

### Take a picture
```
fswebcam -d /dev/video0 -r 1280x720 --no-banner image.jpg
```

```
catimg image.jpg
```

## Disc /Memory SD Card speed test
Writting:
```
dd if=/dev/zero of=testfile bs=4M count=256 conv=fdatasync
```

Reading
```
dd if=testfile of=/dev/null bs=4M
```
