# XFWM-GTK3-DEBIAN-TEAL-THEME  


<a href="url"><img src="https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/assets/102870900/557fb16f-4c9c-4c8a-96ac-94b9f1f59d68" align="center" height="96" width="96" ></a> 
<a href="url"><img src="https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/assets/102870900/3c67318e-2ddb-4cc7-8c5e-b3eea7fdb8f0" align="center" height="96" width="96" ></a>  


A generated GTK3 theme using Skeuos's generator, and a simplistic XFWM theme, that uses the new Debian version of teal (#01a495 - picked out of "/usr/share/images/desktop-base/default"), as well as, thick grabbable borders, large square coloured buttons, a generic title menu button. The XFWM theming is entirely in .XPM text file format.  


## Install  
#### Simply download the ZIP or clone the repository and extract the directory "Skeuos-debian11-Dark" into: "/usr/share/themes/"  
    sudo git clone https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/  
    sudo cp -r xfwm-gtk3-debian-teal-theme/Skeuos-debian11-Dark /usr/share/themes/  
    sudo gio trash --force xfwm-gtk3-debian-teal-theme/  
#### Alternatively, I think you can extract the directory "Skeuos-debian11-Dark" into your own home directory: "~/.local/share/themes/"  
    git clone https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/  
    cp -r xfwm-gtk3-debian-teal-theme/Skeuos-debian11-Dark ~/.local/share/themes/  
    gio trash --force xfwm-gtk3-debian-teal-theme/  


## Uninstall  
#### To uninstall the theme from your system, just remove the directory "Skeuos-debian11-Dark" from "/usr/share/themes/".  
    sudo gio trash --force /usr/share/themes/Skeuos-debian11-Dark  
#### Or remove the directory "Skeuos-debian11-Dark" from your own local files in your home directory in "~/.local/share/themes/".  
    sudo gio trash --force ~/.local/share/themes/Skeuos-debian11-Dark  
#### After removing the directory "Skeuos-debian11-Dark" from the appropriate parent directory, the cache of installed themes needs to be updated. 
#### This can be done by rebooting the system, logging out of your user account, changing your selected theme, or restarting theme related processes:  
    sudo pkill xfce4-panel ; xfce4-panel ; pkill xfwm4 ; xfwm4 --replace ; pkill xfdesktop ; xfdesktop  


## Troubleshooting  
#### To embed the scrollbars into window frames (Disable overlay scrolling). May cause issues with some programs, or not work at all anymore.  
    sudo echo 'GTK_OVERLAY_SCROLLING=0' >> /etc/environment  


## Updates  
Now with appropriately coloured scrollbars. They're also large and square shaped.  


## Update Queue
There are a lot of "OK" buttons with the wrong foreground colours.

