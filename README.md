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

```bash
sudo apt install git
```

安裝 Dependencies: 

```bash
sudo apt install meson dh-autoreconf libxcb-keysyms1-dev libpango1.0-dev libxcb-util0-dev xcb libxcb1-dev libxcb-icccm4-dev libyajl-dev libev-dev libxcb-xkb-dev libxcb-cursor-dev libxkbcommon-dev libxcb-xinerama0-dev libxkbcommon-x11-dev libstartup-notification0-dev libxcb-randr0-dev libxcb-xrm0 libxcb-xrm-dev libxcb-shape0 libxcb-shape0-dev automake libtool xutils-dev autoconf
```

安裝 i3-gaps: 

> 所在位置 ~/
```bash
git clone https://github.com/Airblader/i3 i3-gaps
cd i3-gaps
mkdir -p build && cd build
meson --prefix /usr/local
ninja
sudo ninja install
```

登出就可以選擇 i3 login 了

配置請參考 [i3](config/i3/README.md)

### picom

安裝 Dependencies: 

```bash
sudo apt install libxext-dev libxcb1-dev libxcb-damage0-dev libxcb-xfixes0-dev libxcb-shape0-dev libxcb-render-util0-dev libxcb-render0-dev libxcb-randr0-dev libxcb-composite0-dev libxcb-image0-dev libxcb-present-dev libxcb-xinerama0-dev libxcb-glx0-dev libpixman-1-dev libdbus-1-dev libconfig-dev libgl1-mesa-dev  libpcre2-dev  libevdev-dev uthash-dev libev-dev libx11-xcb-dev libxcb-sync-dev libgl-dev asciidoc
```

安裝 picom

> 所在位置 ~/
```bash
git clone https://github.com/jonaburg/picom.git
cd picom/
git submodule update --init --recursive
meson --buildtype=release . build
ninja -C build
ninja -C build install
```

配置請參考 [picom](config/picom/README.md)

### rofi

安裝 Dependencies: 

```bash
sudo apt install bison flex libxcb-ewmh-dev libgdk-pixbuf2.0-dev
```

配置請參考 [rofi](config/rofi/README.md)

### polybar

安裝 Dependencies

```bash
sudo apt install build-essential git cmake cmake-data pkg-config python3-sphinx python3-packaging libuv1-dev libcairo2-dev libxcb1-dev libxcb-util0-dev libxcb-randr0-dev libxcb-composite0-dev python3-xcbgen xcb-proto libxcb-image0-dev libxcb-ewmh-dev libxcb-icccm4-dev libjsoncpp-dev
```

配置請參考 [polybar](config/polybar/README.md)

### ranger

安裝 Dependencies

```bash
sudo apt install python3 python3-pip
```

配置請參考 [ranger](config/ranger/README.md)

## Fonts

`JetBrainsMono Nerd Font`

[Nerd Font](https://www.nerdfonts.com/font-downloads)

### Install font-manager

好用的字體管理工具 (你會需要的)

```bash
sudo apt install font-manager
```

### Command

使用指令安裝多種字體

> 所在位置 ~/
```bash
mkdir .fonts
cd .fonts
# 把所有要安裝的 ttf 丟到這裡
cd
fc-cache -fv
# 可以使用 font-manager 來確認字體是否安裝成功
```

## Wallpaper
![wallpaper](wallpaper/wallpaper.jpg)

## Reference

* [How to build and install i3-gaps from source on debian](https://lottalinuxlinks.com/how-to-build-and-install-i3-gaps-on-debian/)