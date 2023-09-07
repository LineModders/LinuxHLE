# LinuxHLE
![App Screenshot](Assets/LinuxHLE.png)
A High level linux distro "Ubuntu 20" emulator for android using Termux and VNCserver!
![Screenshot](Assets/ScreenLinuxHLE.png)

# Req
- 4 gb
- termux
- VNCserver

# Installing
- download termux
- download VNCserver
- open termux
- updating ```pkg update``` (write commands)
- install wget ```pkg install wget proot -y```
- copy repo. ```wget https://raw.githubusercontent.com/TypedQue/LinuxHLE/master/ubuntu.sh```
- check file ```ls``` if you see file ubuntu.sh - ok
- bashing ```bash ubuntu.sh```
- ```ls``` if you see 2 new folders - ok
- starting ```./startubuntu.sh```
- Ubuntu install, next, install vnc on Ubuntu
- ```apt update```
- ```rm .bashrc```
- ```cp /etc/skel/.bashrc .```
- ```sed -i 's/32/31/g' .bashrc```
- ```logout```
- ```./startubuntu.sh```
- ```apt install gnome-shell gnome-terminal nautilus gnome-tweaks gnome-shell-extension-ubuntu-dock light-themes suru-icon-theme gedit dbus-x11 tigervnc-standalone-server nano -y``` -installing gnome
- create folder ```mkdir .vnc```
- script ```nano .vnc/xstartup```
- paste this texts -
- ```#!/bin/bash``` enter
- ```export XDG_CURRENT_DESKTOP="GNOME"``` enter
- ```service dbus start``` enter
- ```gnome-shell --x11``` done, save file
- ```chmod +x .vnc/xstartup```
- start vnc ```vncserver -localhost no``` and enter any password
- open vnc
- click plus, in Addres write ```localhost:1```, in name write any name
- done!
- but, for audio. ```pkg install pulseaudio -y```
# Startup
- ```./startubuntu.sh```
- ```vncserver -localhost no``` any password
- open vnc
- open you server
# Shutdown
- ```vncserver -kill :1```

# Authors
- TypedQue (team)
- [@SynthouS](https://youtube.com/SynthouS)
- @Merryweath
