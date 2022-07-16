# Dracula_Mountain

## Cover

### Desktop
![desktop](assets/desktop.png)

### Ranger 1
![picture](assets/picture.png)

### Ranger 2
![ranger](assets/ranger.png)

### Code
![hello](assets/hello.png)

### Lazygit
![lazygit](assets/lazygit.png)

## Tools

* [i3-gaps](https://github.com/Airblader/i3)
* [picom](https://github.com/jonaburg/picom)
* [rofi](https://github.com/davatorium/rofi)
* [polybar](https://github.com/polybar/polybar)

## Installation

Ubuntu 22.04 fresh install.

### i3-gaps

安裝 git

```
sudo apt install git
```

安裝 Dependencies: 

```
sudo apt install meson dh-autoreconf libxcb-keysyms1-dev libpango1.0-dev libxcb-util0-dev xcb libxcb1-dev libxcb-icccm4-dev libyajl-dev libev-dev libxcb-xkb-dev libxcb-cursor-dev libxkbcommon-dev libxcb-xinerama0-dev libxkbcommon-x11-dev libstartup-notification0-dev libxcb-randr0-dev libxcb-xrm0 libxcb-xrm-dev libxcb-shape0 libxcb-shape0-dev automake libtool xutils-dev autoconf
```

Clone && Build: 

```
mkdir clone
cd clone
git clone https://github.com/Airblader/i3 i3-gaps
cd i3-gaps
mkdir -p build && cd build
meson --prefix /usr/local
ninja
sudo ninja install
```

## Wallpaper
![wallpaper](wallpaper/wallpaper.jpg)

## Reference

* [How to build and install i3-gaps from source on debian](https://lottalinuxlinks.com/how-to-build-and-install-i3-gaps-on-debian/)