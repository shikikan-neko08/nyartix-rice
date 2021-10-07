# Nyartix Rice

## i3-gaps

![enter image description here](https://github.com/shikikan-neko08/nyartix-rice/blob/main/assets/2021-09-26-044615_1360x768_scrot.png)

![enter image description here](https://github.com/shikikan-neko08/nyartix-rice/blob/main/assets/2021-09-26-045448_1360x768_scrot.png) 

![enter image description here](https://github.com/shikikan-neko08/nyartix-rice/blob/main/assets/2021-09-26-050612_1360x768_scrot.png)

![enter image description here](https://github.com/shikikan-neko08/nyartix-rice/blob/main/assets/2021-09-26-045031_1360x768_scrot.png)

## BSPWM
![enter image description here](https://github.com/shikikan-neko08/nyartix-rice/blob/main/assets/2021-09-27-090517_1360x768_scrot.png)


# Details
* Font Used : Iosevka Custom
* GTK Theme : Modified version of Lumiere From [addy-dclxvi](https://github.com/addy-dclxvi/gtk-theme-collections) . I'll call it frostneko
* Icons     : Custom Version of papirus (nya)
* OS        : Artix Linux
* WM        : i3-gaps, bspwm
* Terminal  : Kitty
* Shell     : zsh
* Bar       : Polybar
* Lockscreen: betterlockscreen

# Version History
* A-1.0.2       
  Added BSPWM Support
* A-1.0.1      
  New feature: "window move" mode and gap resize mode
* A-1.0      
  Initial release


# To do
* add ~~bspwm~~, herbstluftwm support
* bspwm specific polybar
* urxvt & .Xresources support

# Dependecies
 * [rofi](https://github.com/davatorium/rofi)
 * [kitty](https://github.com/kovidgoyal/kitty)
 * [i3-gaps](https://github.com/Airblader/i3)
 * [bspwm](https://github.com/baskerville/bspwm) (optional)
 * [Polybar](https://github.com/polybar/polybar)
 * [betterlockscreen](https://github.com/pavanjadhaw/betterlockscreen)   
 * nitrogen 
 * Font Awesome
 * [clearine](https://github.com/okitavera/clearine)
 
  Some of this packages might not be available on your distro's repository, please refer to your distro package manager.
  For Arch-based users, you may use AUR for those packages.
  
  > tip : rofi works best on version 1.6.1. if you are using version 1.7.0, it only showing the outline of the selected apps.

# Installation

**Important : Make sure to backup your existing configuration files before installing to avoid loss**     

* Install the dependencies
* Clone this repository
* Install [Starship Prompt](https://starship.rs/)
* Install [powerlevel10k](https://github.com/romkatv/powerlevel10k)
* copy powerlevel10k.zsh-theme to your powerlevel10k folder
* copy .p10k.zsh to your home directory.
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
> betterlockscreen -u /path/to/wallpaper.png

To apply The GTK Theme and icons, you can use LXappearance    

# Basic Keybinding

super key is the windows key      
read more [here](https://en.wikipedia.org/wiki/Super_key_(keyboard_button))

## i3     
Super + Return Terminal     
Super + Shift + Q close     
Super + D rofi     
Super + 1-9 go to workspace x     
Super + Shift + 1-9 move window to workspace x     
Super + R resize mode (use arrows to resize or using wasd)     
Super + Shift + G Toggle gap resizing mode     
Super + Shift + M Toggle move mode 
Super + Left Click move window with drag     
Super + Right Click resize window with drag    
Super + W Toggle tabbing layout       
Super + E Toggle tiling layout     
Super + S Toggle stacking layout     
Super + Shift + Space Toggle Floating mode     
Super + F Toggle Fullscreen     
Super + Shift + E Powermenu (requires clearine)     
Super + Shift + R restart wm     
Super + Escape lockscreen     

## bspwm

Super + Return Terminal     
Super + w close     
Super + space rofi     
Super + 1-9 go to workspace x     
Super + Shift + 1-9 move window to workspace x     
Super + Alt + H, J, K ,L Increase window size       
Super + Alt + Shift + H, J, K ,L Decrease window size    
Super + S Toggle Floating mode     
Super + T Toggle Tiling Mode     
Super + F Toggle Fullscreen     
Super + Alt + Q Powermenu (requires clearine)      
Super + Alt + R restart wm     
Super + Escape restart keybinding     
Super + X lockscreen     

# Issues
> I opened Thunar but it appears to be black theme        

Delete the gtk-dark.css on the theme folder, on gtk3.0


# Notes
* If you are installing this on systemd , don't forget to change the loginctl
 command to systemctl on clearine.conf and polybar config
* Polybar is disabled by default. to enable it run "launchbar" if you are on zsh shell. or uncomment the launch.sh on i3/config. this only affect i3 users. user that using bspwm as their default didn't need to configure this as the polybar is executed during startup


# License

Under MIT License. See ./LICENSE for details.

