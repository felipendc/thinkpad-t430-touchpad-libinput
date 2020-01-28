# Thinkpad-T430-Touchpad libinput and Gestures:

## // Installing libinput: 

1) You need to install "libinput" first: <br />
<pre>sudo pacman -S libinput</pre>


## // Editting 40-libinput.conf file: 

2) Download "40-libinput.conf" to *'/usr/share/X11/xorg.conf.d/40-libinput.conf/'* <br />

<pre>git clone https://github.com/felipendc/thinkpad-t430-touchpad-libinput.git ~/usr/share/X11/xorg.conf.d/40-libinput.conf/ </pre>

3) Or, add these configurations below at the end of your "40-libinput.conf" file at *'/usr/share/X11/xorg.conf.d/40-libinput.conf/'* <br />


<pre>Section "InputClass"
    Identifier "touchpad"
    Driver "libinput"
    MatchIsTouchpad "on"
    Option "Tapping" "on"
EndSection </pre>


## // Installing Touchpad Pinch Gestures : 

4) To install *'libinput-gestures'* we'll use the "Trizen Package Manager"

<pre>trizen -S libinput-gestures</pre>
