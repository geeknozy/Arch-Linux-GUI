# Arch-Linux-GUI
## package list for few good DE/WM on Arch Linux

##### Hyprland window manager <br />
```
pacman -Syu wayland wlroots gcc git meson cairo pango pixman hyprland hyprpaper kitty waybar wofi fastfetch cosmic-files geany lxappearance grim slurp viewnior
```

##### BSPWM a simple beautiful window manager<br />
```
pacman -Syu xorg xorg-xinit bspwm sxhkd xterm rofi polybar picom feh thunar thunar-volman scrot
``` 

##### LXQT Desktop Environment <br />
```
pacman -Syu xorg xorg-xinit lxqt sddm lxappearance kvantum kvantum-qt5 noto-fonts noto-fonts-cjk noto-fonts-emoji ttf-joypixels xcursor-vanilla-dmz
```

##### XFCE4 Desktop Environment <br />
```
pacman -Syu xorg xorg-xinit xfce4 xfce4-terminal xfce4-whiskermenu-plugin xfce4-screenshooter xfce4-pulseaudio-plugin lighdm lightdm-gtk-greeter lightdm-gtk-greeter-settings
```

##### enable ligtdm Display Manager <br />
```
systemctl enable lightdm.service
```

##### Minimal Gnome Desktop Environment <br />
```
pacman -Syu gnome-shell gnome-terminal nautilus gnome-tweaks gnome-control-center gnome-keyring gdm polkit-gnome
```

##### enable gdm display manager <br />
```
systemctl enable gdm.service
```
