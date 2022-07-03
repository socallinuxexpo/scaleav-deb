# SCaLE AV Debian Package

This package contains the necessary setup to build a package for SCaLE AV.

## Building Debian Package

Build this package with `dpgk-deb`.  Current version is 1.0-3.

```
git clone https://github.com/socallinuxexpo/scaleav-deb.git
cd scaleav-deb
./quick-build 1 0 3
```

## Installing Package and Dependencies

```
sudo add-apt-repository ppa:obsproject/obs-studio
sudo apt-get update
sudo apt-get install obs-studio
sudo apt-get install obs-websockets
sudo apt install ./scaleav_1.0-3.deb
```

## Post Installation Configuration

Configuration overlays:

1. `opt/conf/scale.env`: bash environment variable source. Contains needed environment variables.
2. `opt/obs/conf/scale-branding.png`: PNG image used to put branding in videos. 16:9 ratio.
3. `opt/obs/conf/Untitled.json`: fill in "<INSERT-CAMERA-FEED-URL>"
4. `opt/web-control-interface/html/js/config.js`: standard config JS


