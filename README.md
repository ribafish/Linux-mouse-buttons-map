# Linux-mouse-buttons-map

First install:
```
sudo apt-get install xbindkeys xautomation
```

Then do:
```
xbindkeys --defaults > $HOME/.xbindkeysrc
gedit $HOME/.xbindkeysrc
```

### For Logitech Performance MX:
To map Zoom button to middle button paste somewhere:
```
"xte 'mouseclick 2' &"
  b:13 + Release
```

To test current settings:
```
killall xbindkeys && xbindkeys
```

And finally, you need to configure 'xbindkeys' to run automatically on system startup. Startup Applications / Add program button and type '/usr/bin/xbindkeys' on the dialog.

Following this guide:
http://askubuntu.com/questions/19569/how-can-i-assign-actions-to-all-my-mouse-buttons

