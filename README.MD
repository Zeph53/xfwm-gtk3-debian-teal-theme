# XFWM-GTK3-DEBIAN-TEAL-THEME  


# <img src="https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/assets/102870900/557fb16f-4c9c-4c8a-96ac-94b9f1f59d68" height="135" width="240"> <img src="https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/assets/102870900/3c67318e-2ddb-4cc7-8c5e-b3eea7fdb8f0" height="135" width="240">  


A generated GTK3 theme using Skeuos's generator, and a simplistic XFWM theme, that uses the new Debian version of teal (#01a495 - gpick'd out of "/usr/share/images/desktop-base/default"), as well as, thick grabbable borders, large square coloured buttons, a generic title menu button. The XFWM theming is entirely in .XPM text file format. It's really quite performance friendly.  


## Requirements  
This theme was designed for solely Debian-11-Testing (and higher).  
Using XFCE4/GTK3/GTK2 as a desktop environment.  
It can be ported relatively easily, or used as-is in most circumstances.  


## Install  
Simply download the ZIP or clone the repository and extract the directory "Skeuos-debian11-Dark" into:  
#### /usr/share/themes/  
#### Install into system theme directory:  
    sudo git clone https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/
    sudo cp -r xfwm-gtk3-debian-teal-theme/Skeuos-debian11-Dark /usr/share/themes/
    sudo gio trash --force xfwm-gtk3-debian-teal-theme/
Alternatively, I think you can extract the directory "Skeuos-debian11-Dark" into your own home directory:  
#### ~/.local/share/themes/  
#### Install into user's home directory:  
    git clone https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/
    cp -r xfwm-gtk3-debian-teal-theme/Skeuos-debian11-Dark ~/.local/share/themes/
    gio trash --force xfwm-gtk3-debian-teal-theme/
After installing the directory "Skeuos-debian11-Dark" to the appropriate parent directory, the cache of installed themes needs to be updated. This can be achieved by:  
Rebooting the system, logging out of your user account, changing your selected theme, or restarting theme related processes:  
#### Terminate panel, window manager, and desktop processes. Then restart them:  
    sudo pkill xfce4-panel ; xfce4-panel ; pkill xfwm4 ; xfwm4 --replace ; pkill xfdesktop ; xfdesktop


## Uninstall  
To uninstall the theme from your system, just remove the directory "Skeuos-debian11-Dark" from  
"/usr/share/themes/".  
#### Delete theme files from the system:  
    sudo gio trash --force /usr/share/themes/Skeuos-debian11-Dark
Or remove the directory "Skeuos-debian11-Dark" from your own local files in your home directory in  
"~/.local/share/themes/".  
#### Delete theme files from the home directory:  
    gio trash --force ~/.local/share/themes/Skeuos-debian11-Dark
After removing the directory "Skeuos-debian11-Dark" from the appropriate parent directory,  
the cache of installed themes needs to be updated. This can be achieved by rebooting the system,  
logging out of your user account, changing your selected theme, or restarting theme related processes:  
#### Terminate panel, window manager, and desktop processes:  
    sudo pkill xfce4-panel ; xfce4-panel ; pkill xfwm4 ; xfwm4 --replace ; pkill xfdesktop ; xfdesktop


## Troubleshooting  
To embed the scrollbars into window frames (Disable overlay scrolling).  
May cause issues with some programs, or not work at all anymore.  
#### Disable overlay scrollbars:  
    sudo echo 'GTK_OVERLAY_SCROLLING=0' >> /etc/environment
If there are mixmatched foreground or background colours, or any other issues,  
report the issue through the repository issue reporting page on GitHub.  
You may be asked to supply a screenshot of the "CSS Selector" section of "GtkInspector".  
You may need to install "GtkInspector":  
#### Install GTK Development package "libgtk-3-dev":  
    sudo apt install --install-recommends libgtk-3-dev
After installing "GtkInspector", it needs to be enabled within GTK:  
#### Enable "GtkInspector" GTK debugging tool through GSettings:  
    sudo gsettings set org.gtk.Settings.Debug enable-inspector-keybinding true
After installing and enabling the "GtkInspector", while a GTK applcation is focussed,  
simply press "Control-Shift-I" OR "Control-Shift-D". After it opens, on the top left of "GtkInspector"  
click the "Select an Object" icon. Alt-tab to your GTK application with the issue,  
select the highlighted area problem. Navigate to the dropdown menu on the left and select "CSS Selector".  
Screenshot it or take note of all the text for your report.  


## Updates  
Now with appropriately large square shaped coloured scrollbars.  


## Updates Queue  
There are a lot of "OK" buttons with the wrong foreground colours.  


## Issues / Bugs  
#### If there are any bugs, feel free to report them, and they will be added here before going downstream!  


##  
