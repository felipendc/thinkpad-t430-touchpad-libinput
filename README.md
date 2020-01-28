# Thinkpad-T430-Touchpad libinput and Gestures:
![Demo](https://i.imgur.com/fiy4FFX.png)
##

## Installing libinput: 

You need to install "libinput" first: <br />
<pre>sudo pacman -S libinput</pre>


## Downloading the 40-libinput.conf file: 

Download "40-libinput.conf" to *'/usr/share/X11/xorg.conf.d/40-libinput.conf/'* <br />

<pre>sudo git clone https://github.com/felipendc/thinkpad-t430-touchpad-libinput.git ~/usr/share/X11/xorg.conf.d/40-libinput.conf/ </pre>


## Editting 40-libinput.conf file:

Or, add these configurations below at the end of your "40-libinput.conf" file at *'/usr/share/X11/xorg.conf.d/40-libinput.conf/'* <br />


<pre>Section "InputClass"
    Identifier "touchpad"
    Driver "libinput"
    MatchIsTouchpad "on"
    Option "Tapping" "on"
EndSection </pre>

