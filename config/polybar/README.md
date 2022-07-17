# 備註

## Fonts

```bash
mv feather/* ~/.fonts/
mv MaterialIcons/* ~/.fonts/
cd
fc-cache -fv
```

## Clone

> 所在位置 ~/ (務必 clone 在 ~/)
```bash
git clone --depth 1 https://github.com/Murzchnvok/polybar-collection
```

## Replace

替換 `modules.ini`

```bash
rm ~/polybar-collection/modules.ini
mv ./modules.ini ~/polybar-collection/
```
