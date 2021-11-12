# Arch-Linux-GUI
## package list for few good DE/WM on Arch Linux

### Gnome Desktop Environment

```pacman -Syu xorg xorg-xinit gnome-shell gnome-terminal nautilus gnome-tweak-tool gnome-control-center gnome-keyring gdm```

enable gdm display manager

```systemctl enable gdm.service```

### XFCE4 Desktop Environment

```pacman -Syu xorg xorg-xinit xfce4 xfce4-terminal xfce4-whiskermenu-plugin xfce4-screenshooter lighdm lightdm-gtk-greeter lightdm-gtk-greeter-settings```

enable ligtdm Display Manager

```systemctl enable lightdm.service```


#### Optional packages / services etc (universal for all the DE/WM's

```pacman -Syu acpid dbus thermald```

enable the services on startup
```systemctl enable acpid.service```
```systemctl enable dbus.service```
```systemctl enable gdm.service```
```systemctl enable thermald.service```
