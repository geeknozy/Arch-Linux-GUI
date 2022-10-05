# Arch-Linux-GUI
## package list for few good DE/WM on Arch Linux

### XFCE4 Desktop Environment (my favourite)<br />
```
pacman -Syu xorg xorg-xinit xfce4 xfce4-terminal xfce4-whiskermenu-plugin xfce4-screenshooter lighdm lightdm-gtk-greeter lightdm-gtk-greeter-settings
```

#### enable ligtdm Display Manager <br />

```
systemctl enable lightdm.service
```

### BSPWM a simple beautiful window manager<br />
```
pacman -Syu xorg xorg-xinit bspwm sxhkd rxvt-unicode rofi polybar picom feh thunar thunar-volman scrot
``` 

### Gnome Desktop Environment <br />
```
pacman -Syu xorg xorg-xinit gnome-shell gnome-terminal nautilus gnome-tweak-tool gnome-control-center gnome-keyring gdm
```

#### enable gdm display manager <br />
```
systemctl enable gdm.service
```

#### Optional packages / services etc (universal for all the DE/WM's <br /> 
```
pacman -Syu acpid dbus thermald
```

#### enable the services on startup <br />
```
systemctl enable acpid.service
```

```
systemctl enable dbus.service
```

```
systemctl enable thermald.service
```


#### intel graphics related packages
```
pacman -Syu xf86-video-intel intel-ucode libva-intel-driver libva-utils vulkan-intel
```
> Note : xf86-video-intel package is optional as it contains some bugs 

#### misc X11 packages (optional)
```
pacman -Syu xf86-input-libinput xf86-input-evdev libxkbcommon-x11 xcb-util-cursor xcb-util-keysyms xcb-util-renderutil xcb-util-errors
```
