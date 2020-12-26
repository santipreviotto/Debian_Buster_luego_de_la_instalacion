# Debian Buster: instalacion de paquetes

![debian](/debian-logo-1024x576.png)

### Instalar synaptic y intel-microcode

Dentro de una terminal:

`apt install synaptic`

Dentro de synaptic, buscar el paquete "intel-microcode" y el paquete "firmware-atheros" y marcar para instalar.


Reiniciar.

### Instalar paquetes deb

Dentro de una terminal:

```
apt install beignet && apt install gnome-shell-extension-appindicator && apt install build-essential dkms linux-headers-$(uname -r) && apt install ttf-mscorefonts-installer rar unrar libavcodec-extra gstreamer1.0-libav gstreamer1.0-plugins-ugly gstreamer1.0-vaapi && apt install freecad && apt install gimp && apt install octave && apt install inkscape && apt install kicad && apt install telegram-desktop
```

### Instalar flatpak, discord, okular, spotify y zoom

Dentro de una terminal:

`apt install flatpak`

Luego:

```
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

Reiniciar.
