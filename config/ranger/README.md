# 備註

* 生成 ranger config files
* 啟用 preview highlight
* 安裝 ranger icons
* 啟用 preview image

## 生成 ranger config files

```bash
ranger --copy-config=all
```

## 安裝 pygments dracula highlight

```bash
git clone https://github.com/dracula/pygments.git
cd pygments/
sudo mv dracula.py /usr/lib/python3/dist-packages/pygments/styles/
# TODO: 想辦法不用 sodo 就能讓 pygments 讀取 dracula.styles
```

### 啟用 highlight

請參考 [scope.sh](scope.sh) 內的內容

## 安裝 ranger icons

```bash
git clone https://github.com/alexanderjeurissen/ranger_devicons ~/.config/ranger/plugins/ranger_devicons
echo "default_linemode devicons" >> $HOME/.config/ranger/rc.conf
```

### 啟用 preview image

請參考 [rc.conf](rc.conf) 內的內容
