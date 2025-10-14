# Arch-Linux-GUI
## package list for few good DE/WM on Arch Linux

##### Hyprland window manager <br />
```
pacman -Syu wayland wlroots gcc git meson libxcbcommon cairo pango pixman hyprland hyprpaper kitty waybar rofi fastfetch nautilus geany
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
pacman -Syu xorg xorg-xinit gnome-shell gnome-terminal nautilus gnome-tweak-tool gnome-control-center gnome-keyring gdm
```

##### enable gdm display manager <br />
```
systemctl enable gdm.service
```

##### Optional packages / services etc (
> these packages are universal for all the DE/WMs, ie: you can use these with any DE or WMs <br /> 
```
pacman -Syu acpid dbus thermald tlp
```

##### enable the services on startup <br />
```
systemctl enable acpid.service
```

```
systemctl enable dbus.service
```

```
systemctl enable thermald.service
```

```
systemctl enable tlp.service
```


##### intel graphics related packages
> if you observe screen tearing issue on intel based integrated GPU check this link -> [intel screen tear resolve](https://github.com/geeknozy/linux-screen-tear-resolve).
```
pacman -Syu xf86-video-intel intel-ucode libva-intel-driver libva-utils vulkan-intel xf86-video-amdgpu
```
> Note : xf86-video-intel package is optional as it contains some bugs 

##### misc X11 packages (optional)
```
pacman -Syu xf86-input-libinput xf86-input-evdev libxkbcommon-x11 xcb-util-cursor xcb-util-keysyms xcb-util-renderutil xcb-util-errors
```
