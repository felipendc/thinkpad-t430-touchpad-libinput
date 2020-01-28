# Thinkpad-T430-Touchpad-libinput:

1) You need to install "libinput" first:
sudo pacman -S libinput

2) Download "40-libinput.conf" to "/usr/share/X11/xorg.conf.d/40-libinput.conf/"

3) Or, add these configurations below at the end of your "40-libinput.conf" file at "/usr/share/X11/xorg.conf.d/40-libinput.conf/"


Section "InputClass"
    Identifier "touchpad"
    Driver "libinput"
    MatchIsTouchpad "on"
    Option "Tapping" "on"
EndSection


