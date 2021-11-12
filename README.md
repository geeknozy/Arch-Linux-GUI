# Arch-Linux-GUI
## package list for few good DE/WM on Arch Linux

### Gnome Desktop Environment <br />

```pacman -Syu xorg xorg-xinit gnome-shell gnome-terminal nautilus gnome-tweak-tool gnome-control-center gnome-keyring gdm```

enable gdm display manager <br />

```systemctl enable gdm.service```

### XFCE4 Desktop Environment <br />

```pacman -Syu xorg xorg-xinit xfce4 xfce4-terminal xfce4-whiskermenu-plugin xfce4-screenshooter lighdm lightdm-gtk-greeter lightdm-gtk-greeter-settings```

enable ligtdm Display Manager <br />

```systemctl enable lightdm.service```


#### Optional packages / services etc (universal for all the DE/WM's <br /> 

```pacman -Syu acpid dbus thermald```

enable the services on startup <br />
```systemctl enable acpid.service```<br />
```systemctl enable dbus.service```<br />
```systemctl enable thermald.service```<br />
