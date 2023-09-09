# LinuxHLE
![App Screenshot](Assets/LinuxHLE.png)
A High level linux distro "Ubuntu 20" emulator for android using Termux and VNCserver!
![Screenshot](Assets/ScreenLinuxHLE.png)

# Req
- 4 gb
- termux
- RealVNC

# Installing
- open termux
- updating ```pkg update``` (write commands)
- install wget ```pkg install wget proot -y```
- copy repo. ```wget https://raw.githubusercontent.com/TypedQue/LinuxHLE/master/ubuntu.sh```
- bashing ```bash ubuntu.sh```
- starting ```./startubuntu.sh```
- Ubuntu install, next, install vnc and gnome on Ubuntu
- ```./startubuntu.sh```
- ```apt update```
- ```apt install gnome-shell gnome-terminal nautilus gnome-tweaks gnome-shell-extension-ubuntu-dock light-themes suru-icon-theme gedit dbus-x11 tigervnc-standalone-server nano -y``` - installing gnome
- gnome starting script ```wget https://raw.githubusercontent.com/TypedQue/LinuxHLE/master/xstartuplh```
- ```chmod +x xstartuplh```
- start vnc ```vncserver -localhost no``` and enter any password
- open RealVNC
- click plus, in Addres write ```localhost:1```, in name write any name
- done!
# Startup
- ```./startubuntu.sh```
- ```chmod +x xstartuplh```
- ```vncserver -localhost no``` any password
- open vnc
- open you server
# Shutdown
- ```vncserver -kill :1```

# Authors
- TypedQue (team)
- [@SynthouS](https://youtube.com/SynthouS)
- @Merryweath
