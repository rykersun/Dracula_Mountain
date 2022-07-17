# 備註

## 註解

* 請先將 [config](config) 裡面標示要註解的項目註解
* 將 [config](config) 的內容加入到 `~/.config/i3/config` 裡面

## feh

安裝 `feh`: 

```bash
sudo apt install feh
```

將 [config](config) 第 54 行的 sun 改成自己的使用者名稱

將桌布命名成 `wallpaper.jpg` (或著[直接下載 Dracula_Mountain 的桌布](../../wallpaper/wallpaper.jpg))

將桌布放到圖片資料夾

### 建立圖片捷徑

使用指令建立圖片資料夾的連結: 

```bash
ln -s ~/圖片 pictures
```

## 螢幕截圖

安裝 `maim`: 

```bash
sudo apt install maim
```

參考上面建立 `pictures`