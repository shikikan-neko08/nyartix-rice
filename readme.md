# Nyartix Rice

![enter image description here](https://github.com/shikikan-neko08/nyartix-rice/blob/main/assets/2021-09-26-044615_1360x768_scrot.png)

![enter image description here](https://github.com/shikikan-neko08/nyartix-rice/blob/main/assets/2021-09-26-045448_1360x768_scrot.png) 

![enter image description here](https://github.com/shikikan-neko08/nyartix-rice/blob/main/assets/2021-09-26-050612_1360x768_scrot.png)

![enter image description here](https://github.com/shikikan-neko08/nyartix-rice/blob/main/assets/2021-09-26-045031_1360x768_scrot.png)




# Details
* Font Used : Iosevka Custom
* GTK Theme : Modified version of Lumiere From [addy-dclxvi](https://github.com/addy-dclxvi/gtk-theme-collections) . I'll call it frostneko
* Icons     : Custom Version of papirus (nya)
* OS        : Artix Linux
* WM        : i3-gaps
* Terminal  : Kitty
* Shell     : zsh
* Bar       : Polybar
* Lockscreen: betterlockscreen

# Version History

* A-1.0.1      
  New feature: "window move" mode and gap resize mode
* A-1.0      
  Initial release


# To do
* add bspwm, herbstluftwm support
* urxvt & .Xresources support

# Dependecies
 * [rofi](https://github.com/davatorium/rofi)
 * [kitty](https://github.com/kovidgoyal/kitty)
 * [i3-gaps](https://github.com/Airblader/i3)
 * [Polybar](https://github.com/polybar/polybar)
 * [betterlockscreen](https://github.com/pavanjadhaw/betterlockscreen)   
 * nitrogen 
 * Font Awesome
 * [clearine](https://github.com/okitavera/clearine)

# Installation

**Important : Make sure to backup your existing configuration files before installing to avoid loss**     

* Install the dependencies
* Clone this repository
* Install [Starship Prompt](https://starship.rs/)
* Install [powerlevel10k](https://github.com/romkatv/powerlevel10k)
* copy powerlevel10k.zsh-theme to your powerlevel10k folder
* install the required fonts by copying .fonts directory to your home directory      
> **Note : for Source han and ttf-font-awesome, install it from your repository**          
> **Arch : sudo pacman -S adobe-source-han-sans-jp-fonts ttf-font-awesome**
* copy all .config files to your .config directory
* copy all .themes, .icons folders to your home directory
* install oh-my zsh then manually then move .zshrc into your home directory
* install pywal and move .cache/wal into your .cache directory
* install [vim-plug](https://github.com/junegunn/vim-plug)
* copy vimrc into .vim directory
* manually install the plug by opening vimrc using vim then instal the plugin using :PlugInstall   
* Set the wallpaper using nitrogen  
* Set Lockscreen Wallpaper using this command      
> betterlockscreen -u /path/to/wallpaper_kaga.png

To apply The GTK Theme and icons, you can use LXappearance    


# Notes
* If you are installing this on systemd , don't forget to change the loginctl
 command to systemctl on clearine.conf and polybar config
* Polybar is disabled by default. to enable it run "launchbar" if you are on zsh shell. or uncomment the launch.sh on i3/config

