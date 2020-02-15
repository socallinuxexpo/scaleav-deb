# SCaLE AV Debian Package

This package contains the necessary setup to build a package for SCaLE AV.

Build this package with `dpgk-deb`.  Current version is 1.0-2.

```
git clone https://github.com/socallinuxexpo/scaleav-deb.git scaleav_1.0-2 
dpkg-deb --build scaleav_1.0-2/
```

Configuration overlays:

1. `opt/obs/conf/obs.env`: bash environment variable source. Contains the X display for
obs, home directory for OBS, and the URL to stream to logged-disk.
2. `opt/obs/conf/scale-branding.png`: PNG image used to put branding in videos. 16:9 ratio.
3. `opt/obs/conf/Untitled.json`: fill in "<INSERT-CAMERA-FEED-URL>"
4. `opt/web-control-interface/html/js/config.js`: standard config JS


