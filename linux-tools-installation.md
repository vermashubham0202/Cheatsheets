# Software installation:
## Media Player:
```
sudo apt-get install vlc
```
## Camera:
```
sudo apt-get install cheese
```
## Pdf Reader:
```
sudo apt-get install okular
```
or
```
sudo apt-get install evince
```
## Youtube downloader:
```
sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
```
```
sudo chmod a+rx /usr/local/bin/youtube-dl
```
If you do not have curl, you can alternatively use a recent wget:
``` 
sudo wget https://yt-dl.org/downloads/latest/youtube-dl -O /usr/local/bin/youtube-dl
```
```
sudo chmod a+rx /usr/local/bin/youtube-dl
```
## Text Editor:
```
sudo apt-get install gedit
```
## Install R:
```
sudo apt-get install r-base
```
## Install woeusb:
```
sudo add-apt-repository ppa:nilarimogard/webupd8
```
```
sudo apt update
```
```
sudo apt install woeusb
```
## Image viewer:
```
sudo apt-get install nomacs
```
## Java21:
```
sudo apt-get install openjdk-21-jdk
```
## Java21 documentation:
```
sudo apt-get install openjdk-21-source
```
(location : /usr/lib/jvm/openjdk-21/src.zip)
## Archive manager:
```
sudo apt-get install xarchiver
```
## To manage main menu:
```
sudo apt-get install alacarte
```
## PHP installation:
```
sudo apt-get install php
```
```
sudo apt-get install libapache2-mod-php
```
## Apache webserver installation:
```
sudo apt-get install apache2
```
(sudo /etc/init.d/apache2 [start/stop/restart])
## Sqlite database gui installation:
```
sudo apt-get install sqlitebrowser
```
## Sqlite non-gui:
```
sudo apt-get install sqlite3 libsqlite3-dev
```
## Mysql client installation:
```
sudo apt-get install mysql-client
```
## Mysql server installation:
```
sudo apt-get install mysql-server
```
For PHP MyAdmin also install these:
```
sudo apt-get install libapache2-mod-auth-mysql
```
```
sudo apt-get install php5-mysql phpmyadmin
```
## ifconfig command installation:
```
sudo apt-get install net-tools
```
## Debian sudo installation:
```
su-
```
```
apt-get install sudo -y
```
```
usermod -aG sudo yourusername
```
(Open visudo and type following in the last line if this line is missing):
```
%yourusername ALL=(ALL:ALL) ALL
```
## PlayOnLinux installation (To run Windows Applications):
```
sudo apt-get install playonlinux
```
## Dell Latitude (Debian) Wifi driver:
```
apt update && apt install firmware-iwlwifi
```
```
modprobe -r iwlwifi ; modprobe iwlwifi
```
## Sony vaio (Debian) Wifi driver:
### Debian 10 "Buster" (add below line in sources.list)
```
deb http://deb.debian.org/debian buster-backports main contrib non-free
```
After that run below commands:
```
apt-get update
```
```
apt-get install linux-image-$(uname -r|sed 's,[^-]*-[^-]*-,,') linux-headers-$(uname -r|sed 's,[^-]*-[^-]*-,,') broadcom-sta-dkms
```
```
modprobe -r b44 b43 b43legacy ssb brcmsmac bcma
```
```
modprobe wl
```	
## Dell Inspiron i3 Wifi driver:
```
sudo apt-get install firmware-atheros
```
## Disks tool linux:
```
sudo apt-get install gnome-disk-utility
```
## Calculator:
```
sudo apt-get install gnome-calculator
```
## Calender:
```
sudo apt-get install gnome-calendar
```
## Team-viewer dependencies:
```
sudo apt-get install geoclue-2.0 iio-sensor-proxy libqt5positioning5 libqt5sensors5 libqt5webchannel5 libqt5webkit5 qml-module-qtgraphicaleffects qml-module-qtquick-controls qml-module-qtquick-dialogs qml-module-qtquick-layouts qml-module-qtquick-privatewidgets qml-module-qtquick-window2 qml-module-qtquick2
```
## Nvidia installation:
```
sudo apt-get install nvidia-detect 
```
```
sudo apt-get install nvidia-driver
```
## Scanner Tool:
```
sudo apt-get install simple-scan
```
## Audio Video Editing Tool:
```
sudo apt-get install kdenlive
```
## Debian package installer:
```
sudo apt-get install gdebi
```
## Git:
```
sudo apt-get install git
```
## Deleted file recovery tool (Support all extensions recovery):
```
sudo apt-get install testdisk
```
## Image editor:
```
sudo apt-get install gimp
```
## rename command linux:
```
sudo apt-get install rename
```
## tree command linux:
```
sudo apt-get install tree
```
## Bluetooth Manager driver:
```
sudo apt-get install blueman
```
## Processor driver:
### For Intel Processor:
```
sudo apt-get install intel-microcode
```
### For AMD Processor:
```
sudo apt-get install amd64-microcode
```
## playonlinux office 2007 fix:
```
sudo rm -rf Office2007
```
```
sudo dpkg --add-architecture i386
```
```
sudo wget -nc -O /usr/share/keyrings/winehq-archive.key https://dl.winehq.org/wine-builds/winehq.key
```
```
sudo wget -nc -P /etc/apt/sources.list.d/ https://dl.winehq.org/wine-builds/ubuntu/dists/focal/winehq-focal.sources
```
```
sudo apt install --install-recommends winehq-stable
```
```
wine --version
```

# Important Links:
## Debian sources.list generator:
```
https://debgen.simplylinux.ch
```
## System image:
```
https://www.wikihow.com/Create-a-Disk-Image-from-a-Linux-System-Using-Systemback
```
## Sweet Home 3D Models:
```
http://www.sweethome3d.com/freeModels.jsp
```	
## AWS Login Command:
```
chmod 440 security-key.pem
```
```
ssh -i security-key.pem shubham@ec2-13-233-206-224.ap-south-1.compute.amazonaws.com 
```
## To set 'prt sc' button for screenshot in xfce:
Go to : Settings -> Keyboard -> Application Shortcut
Create new shortcut : "xfce4-screenshooter -f" and press PrtSc button.
## Eclipse root issue fix:
```
sudo chmod 775 -R /root/
```
