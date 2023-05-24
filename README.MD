# XFWM-GTK3-DEBIAN-TEAL-THEME  

A generated GTK3 theme using Skeuos's generator and a XFWM theme, that uses the new Debian version of teal  
(#01a495 - picked out of "/usr/share/images/desktop-base/default"), as well as, thick grabbable borders,  
large square coloured buttons, a generic title menu button, simply in .XPM text format.  


## Install  
#### Simply download the ZIP or clone the repository and extract the directory "Skeuos-debian11-Dark" into: "/usr/share/themes/"  
    sudo git clone https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/  
    sudo cp -r xfwm-gtk3-debian-teal-theme/Skeuos-debian11-Dark /usr/share/themes/  
#### Alternatively, I think you can extract the directory "Skeuos-debian11-Dark" into your own home directory: "~/local/share/themes/"  
    git clone https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/  
    cp -r xfwm-gtk3-debian-teal-theme/Skeuos-debian11-Dark /local/share/themes/  


## Uninstall  
#### To uninstall the theme from your system, just remove the directory "Skeuos-debian11-Dark" from "/usr/share/themes/".  
    sudo gio trash --force /usr/share/themes/Skeuos-debian11-Dark  
#### Or remove the directory "Skeuos-debian11-Dark" from your own local files in your home directory in "~/local/share/themes/".  
    sudo gio trash --force ~/local/share/themes/Skeuos-debian11-Dark  
#### After removing the directory "Skeuos-debian11-Dark" from the appropriate parent directory, the cache of installed themes needs to be updated.  
This can be done by rebooting the system, logging out of your user account, changing your selected theme, or execute this one-liner to  
restart theme related processes:  
    sudo pkill xfce4-panel ; xfce4-panel ; pkill xfwm4 ; xfwm4 --replace ; pkill xfdesktop ; xfdesktop


## Troubleshooting  
#### Run this command to embed the scrollbars into window frames (Disable overlay scrolling). May cause issues with some programs, or not work at all anymore.  
    sudo echo 'GTK_OVERLAY_SCROLLING=0' >> /etc/environment  


## Updates  
Now with appropriately coloured scrollbars. They're also YUGE.  
