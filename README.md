## feriado
Python script for [polybar](https://github.com/polybar/polybar) that shows next holiday in Argentina.

![](screenshot.png)

### My polybar
![](polybar.png)


Theme from [polybar-themes](https://github.com/adi1090x/polybar-themes#-polybar-12).

### Install
Add custom script module in polybar config.

```
[module/feriado]
type = custom/script
exec = $HOME/.scripts/feriado -f
interval = 43200   # update each 12 hours
click-left = $HOME/.scripts/feriado -i
click-right = dunstify $($HOME/.scripts/feriado -m)
```

### Options
```
usage: feriado [-h] [-f] [-i] [--open-info] [-m]

optional arguments:
  -h, --help    show this help message and exit
  -f, --fecha   Muestra la fecha del feriado
  -i, --info    Muestra la URL a la información sobre el feriado
  --open-info   Abre la URL de la info en el navegador
  -m, --motivo  Muestra el motivo del feriado
```
