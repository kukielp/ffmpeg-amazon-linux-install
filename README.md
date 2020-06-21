# ffmpeg-amazon-linux-install
How to install ffmpeg on Amazon Linux


```bash
#!/bin/bash

cd /usr/local/bin
mkdir ffmpeg

cd ffmpeg
wget https://johnvansickle.com/ffmpeg/releases/ffmpeg-release-amd64-static.tar.xz
tar xvf ffmpeg-release-amd64-static.tar.xz
rm -rf /usr/local/bin/ffmpeg/ffmpeg-release-amd64-static.tar.xz
folder=$(ls)
mv $folder/ffmpeg .
rm -rf $folder
ln -s /usr/local/bin/ffmpeg/ffmpeg /usr/bin/ffmpeg
```
