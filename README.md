# MyConfiguracion
Mi configuracion de i3 y polybar.

<p align="center">
  <img src="imagen.png" alt="Polybar">
</p>

## clonamos el repo

```
$ cd ~
$ git clone https://github.com/Gilgamesh06/MyConfiguracion.git
```

## Instalacion de los temas.

<p>
	debera descomprimir los arhivos y luego moverlos los temas descargados a las capertas pertinentes
</p>

```
$ cd ~/MyConfiguracion/ 
$ tar -xzvf "nombre de losr archivos con extencion"
$ mv ~/MyConfiguracion/themas/thema/trollwut-pink-dark /usr/share/themes/
$ mv ~/MyConfiguracion/themas/iconos/Simply-Pink-Circles /usr/share/icons
$ mv ~/MyConfiguracion/themas/rofi/solarized-darker.rasi /usr/share/rofi/themes
```

## Administrar temas

<p>
	Para ello primero instalarelos: 
</p>

### Debian o derivados 

```
$ sudo apt-get install lxappearance
```

### fedora 

```
$ sudo dnf install lxappearance
```

## Compton

```
$ mv ~/MyConfiguracion/compton  ~/.config
```

## Polybar 

**Si no tiene instalado polybar**
 

### Dependencias 

### Debian o derivados 

```
$ apt install build-essential git cmake cmake-data pkg-config python3-sphinx libcairo2-dev libxcb1-dev libxcb-util0-dev libxcb-randr0-dev libxcb-composite0-dev python3-xcbgen xcb-proto libxcb-image0-dev libxcb-ewmh-dev libxcb-icccm4-dev

```
```
$ apt install libxcb-xkb-dev libxcb-xrm-dev libxcb-cursor-dev libasound2-dev libpulse-dev i3-wm libjsoncpp-dev libmpdclient-dev libcurl4-openssl-dev libnl-genl-3-dev

```

### fedora 


```
$ sudo dnf install -y cairo-devel xcb-util-devel libxcb-devel xcb-proto xcb-util-image-devel xcb-util-wm-devel
```
```
$ sudo dnf install -y xcb-util-xrm-devel xcb-util-cursor-devel alsa-lib-devel pulseaudio-libs-devel i3-ipc jsoncpp-devel libmpdclient-devel libcurl-devel wireless-tools-devel libnl3-devel

```
## Instalacion polybar 


<p>
	Si su distro tiene paquete no tiene que instalarlo manual
	consulte : https://github.com/polybar/polybar
</p>

<p>
	Descarge el archivo .tar de : https://github.com/polybar/polybar/releases 
</p>


``` 
$ tar -xzvf "el archivo descargado con extencion"
```
```
$ mkdir build
$ cd build
$ cmake ..
$ make -j$(nproc)
$ sudo make install
```
### Tema polybar

```
$ mv ~/MyConfiguracion/polybar  ~/.config
```

## i3

**Si no a instalado i3**

### Debian derivados


```
$ sudo apt-get install i3
```

### Fedora

```
$ sudo dnf install i3

```

### i3 archivo


```
$ cd ~/.i3
$ rm config
$ mv ~/MyConfiguracion/.i3/config  ~/.config

```

**Fondo de pantalla**

*Si desea cambiarlo edite la **linea 37** del archivo config de que esta en la carpeta `~/.i3`*