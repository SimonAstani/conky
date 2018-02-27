# conky
1. apt-get install conky, conky-all
    man conky
2. apt-get install conky-manager
3. /etc/conky/conky.conf= > default script which gets run..
4. edit the scripts as desired..
5. we need to run the script when os boot

Mulitple conky two methods.
Why this solution is best. we may find other conky .. and installation scripts. but the confugration made to the one computer cannot run to other. so, customize the content. The process is confusing.
=================GUI BASED METHODS=================
5. Conky-manager allows multiple scripts at once..
6. Download the files content script  and paste it to other any scripts../
7. make conky-manager in auto-start mode.
8. Tick the conky that you want to made...

===============Creating own autostart scripts====================
1. gedit //bin/conky_start
2. -#!/bin/bash
    conky -c ~/.conky/.conkyrc_top &
    conky -c ~/.conky/.conkyrc_bottom

3. chmod a+x ~/bin/conky_start
4. alt+f2 = conky_start add
5. conky_Start cmd

 wget https://github.com/hant0508/startup-settings/raw/master/debian/startup-settings-amd64.deb 

 sudo dpkg -i startup-settings-amd64.deb 

 add application cmd..

 or create custom /home/.config/autostart ==> crate custom scripts conky_start.desktop

[Desktop Entry]
Name=conky_start
Comment=Run conky_start
Exec=conky_start
Terminal=false
Type=Application