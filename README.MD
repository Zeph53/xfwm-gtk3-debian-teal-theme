github forcing the use of 2fa now. i don't own a cellphone and i won't be buying one just to create free stuff.
i won't be relying on third party password managers, or less-than-functional authentication apps either.

it was an interesting run on gitHub for like 7 years. 
not a single comment, reaction, issue report, star, feedback of any kind..
still tried sending things out there..

if i can't access any of the stuff that i've made due to github's forcing of 2fa, then none of you can either.




## XFWM-GTK3-DEBIAN-TEAL-THEME  


<img src="https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/assets/102870900/557fb16f-4c9c-4c8a-96ac-94b9f1f59d68" height="135" width="240"> <img src="https://github.com/Zeph53/xfwm-gtk3-debian-teal-theme/assets/102870900/3c67318e-2ddb-4cc7-8c5e-b3eea7fdb8f0" height="135" width="240">  


A generated GTK3 theme using Skeuos's generator, and a simplistic XFWM theme, that uses the new Debian version of teal (#01a495 - gpick'd out of "/usr/share/images/desktop-base/default"), as well as, thick grabbable borders, large square coloured buttons, a generic title menu button. The XFWM theming is entirely in .XPM text file format. It's really quite performance friendly.  


## Requirements  
This theme was designed for solely Debian-11-Testing (and higher).  
Using XFCE4/GTK3/GTK2 as a desktop environment. It can be ported relatively easily, or used as-is in most circumstances. As well as a resolution of 1920x1080, which may not be required. The xfce4-panel with this theme is currently designed for these settings in mind: 1 horizontal row, row size 32px, icon size 32px.  


## Installation  
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
After installing the directory "Skeuos-debian11-Dark" to the appropriate parent directory, the cache of installed themes needs to be updated.  
This can be achieved by:  
Rebooting the system, logging out of your user account, changing your selected theme, or restarting theme related processes.  
#### Terminate panel, window manager, and desktop processes. Then restart them:  
    sudo pkill xfce4-panel ; xfce4-panel ; pkill xfwm4 ; xfwm4 --replace ; pkill xfdesktop ; xfdesktop


## Uninstallation  
To uninstall the theme from your system, just remove the directory "Skeuos-debian11-Dark" from:  
#### /usr/share/themes/  
#### Delete theme files from the system:  
    sudo gio trash --force /usr/share/themes/Skeuos-debian11-Dark
Or remove the directory "Skeuos-debian11-Dark" from your own local files in your home directory in:  
#### ~/.local/share/themes/  
#### Delete theme files from the home directory:  
    gio trash --force ~/.local/share/themes/Skeuos-debian11-Dark
After uninstalling the directory "Skeuos-debian11-Dark" from the appropriate parent directory, the cache of installed themes needs to be updated.  
This can be achieved by:  
Rebooting the system, logging out of your user account, changing your selected theme, or restarting theme related processes.  
#### Terminate panel, window manager, and desktop processes. Then restart them:  
    sudo pkill xfce4-panel ; xfce4-panel ; pkill xfwm4 ; xfwm4 --replace ; pkill xfdesktop ; xfdesktop


## Troubleshooting  
GTK3 uses overlay scrollbars, they get in the way sometimes, a preferable scrollbar would be embedded into window frames.  
To embed the scrollbars into window frames (Disable overlay scrolling), GTK3 needs overlay scrollbars disabled, which may cause issues with some applications, or not function at all anymore.  
#### Disable overlay scrollbars:  
    sudo echo 'GTK_OVERLAY_SCROLLING=0' >> /etc/environment
If there are mixmatched foreground or background colours, or any other issues, report the issue through the repository issue reporting page on GitHub.  
You may be asked to supply a screenshot of the "CSS Selector" section of "GtkInspector".  
You may need to install "GtkInspector":  
#### Install GTK3 Development package "libgtk-3-dev":  
    sudo apt install --install-recommends libgtk-3-dev
After installing "GtkInspector", it needs to be enabled within GTK3:  
#### Enable "GtkInspector" GTK3 debugging tool through GSettings:  
    sudo gsettings set org.gtk.Settings.Debug enable-inspector-keybinding true
After installing and enabling the "GtkInspector", while a GTK3 applcation is focussed:  
Simply press "Control-Shift-I" OR "Control-Shift-D".  
After it opens, on the top left of "GtkInspector" click the "Select an Object" icon.  
Alt-tab to your GTK3 application with the issue, select the highlighted area problem.  
Navigate to the dropdown menu on the top left of "GtkInspector" and select "CSS Selector".  
Screenshot it (ALT-PrintScreen) or take note of all the text for your report.  


## Updates  
Fixed window button width for 1920x1080
Many corrections to the README.MD.  
Created a readable README.MD.  
Now with appropriately large square shaped coloured scrollbars.  


## Updates Queue  
Corrections to the XFCE4 Panel theme.  Such as background colour on the workspace widget.  
Ongoing touchups to README.MD.  
There are a lot of "OK" buttons with the wrong foreground colours.  


## Issues / Bugs  
#### If there are any bugs, feel free to report them, and they will be added here before going downstream!  


##  
