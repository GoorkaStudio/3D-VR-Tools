# USB camera
Raspberry Pi / DietPi / NanoPi

# Video
## instalation
```
sudo apt update
sudo apt install ffmpeg
```

## Recording
Best performance (low dropped frames) - 1h of recording create ~3GB file.
`ffmpeg -f v4l2 -framerate 10 -video_size 800x600 -i /dev/video0 -c:v libx264 -preset ultrafast -t 1:00:00 output.mp4`


## Takie picture/jpg



## Disc /Memory SD Card speed test
Writting:
`dd if=/dev/zero of=testfile bs=4M count=256 conv=fdatasync`

Reading
`dd if=testfile of=/dev/null bs=4M`
