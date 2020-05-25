# INSTALLING TOUCHSCREEN 3.5" TO RASPBERRYpi 3B+

### Clear old libraries (if exists)
* sudo rm -rf LCD-show

### Get the repo
* git clone  https://github.com/goodtft/LCD-show.git

### Give exec permission
* chmod -R 755 LCD-show

### Launch the script for the installation
* cd LCD-show/
* sudo ./LCD35-show

## After installed, 
* sudo nano /etc/X11/xorg.conf.d/99-calibration.conf

## add this two lines just before "EndSection"
* Option "InvertY" "true"
* Option "InvertX" "true"

## Finally, reboot.
* reboot
