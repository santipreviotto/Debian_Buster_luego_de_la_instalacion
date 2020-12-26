# Debian Buster: Pasos a seguir luego de la instalación

![debian](/debian-logo-1024x576.png)

### Configurar Software & Updates

Dentro de Software & Updates tildar las casillas como lo describe la ilustración siguiente:

![software&updates](/C1.png)

### Cambiar a los repositorios correctos

Dentro de un terminal:

`sudo nano /etc/apt/sources.list`

Comentar todas las líneas con el caracter # al principio de cada una y copiar la nueva lista de repositorios extraídos desde la página web Sources List Generator:

```
deb http://deb.debian.org/debian/ stable main contrib non-free

deb http://deb.debian.org/debian/ stable-updates main contrib non-free

deb http://deb.debian.org/debian-security stable/updates main

deb http://ftp.debian.org/debian buster-backports main
``` 
Luego dentro de la terminal actualizar el sistema:

`apt update`

### Cambiar la sesión a Xorg

Al iniciar sesión se puede cambiar mediante el símbolo de configuracion y seleccionar "System X11 Default".

![xorg](/C2.jpeg)

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

### Instalar paquetes deb como megasync y VNCViewer 

Entrar a la web de cada uno y descargar el archivo .deb. Luego dentro de una terminal:

`apt install /home/sp/Descargas/nombredelarchivodescargado.deb`
 
### Instalar flatpak, discord, okular, spotify y zoom

Dentro de una terminal:

`apt install flatpak`

```
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

Reiniciar.
