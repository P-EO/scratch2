# scratch2

Install Scratch 2 back on the latest Raspberry Pi OS. They decided to remove Scratch 2 after Adobe Flash was discontinued.  
Fortunately, it's pretty easy to install back.

## To install
[![badge](https://github.com/Botspot/pi-apps/blob/master/icons/badge.png?raw=true)](https://github.com/Botspot/pi-apps)  
Or, to install manually:
```
git clone https://github.com/Botspot/scratch2
sudo cp -af ~/scratch2/libpepflashplayer.so /usr/lib/chromium-browser/libpepflashplayer.so
sudo apt install -yf ~/scratch2/scratch2_0.25_armhf.deb
rm -rf ~/scratch2
```
Scratch 2 package acquired from [the official archive page](http://archive.raspberrypi.org/debian/pool/main/s/scratch2/).  
The `libpepflashplayer.so` file was snatched from an old Raspbian image.
