# Thinkpad-T430-Touchpad-libinput:

## // Installing libinput: 

1) You need to install "libinput" first: <br />
- sudo pacman -S libinput <br />


## // Editting 40-libinput.conf file: 

2) Download "40-libinput.conf" to *'/usr/share/X11/xorg.conf.d/40-libinput.conf/'* <br />

3) Or, add these configurations below at the end of your "40-libinput.conf" file at *'/usr/share/X11/xorg.conf.d/40-libinput.conf/'* <br />


<pre>Section "InputClass"
    Identifier "touchpad"
    Driver "libinput"
    MatchIsTouchpad "on"
    Option "Tapping" "on"
EndSection </pre>


