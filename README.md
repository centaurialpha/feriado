## feriado
Show next holiday information in Argentina. It can be used as a "module" in Polybar or Qtile.

![](screenshot.png)

### Polybar
![](polybar.png)


Add custom script module in polybar config.

```
[module/feriado]
type = custom/script
exec = $HOME/.scripts/feriado -f
interval = 43200   # update each 12 hours
click-left = $HOME/.scripts/feriado -i
click-right = dunstify $($HOME/.scripts/feriado -m)
```

Theme from [polybar-themes](https://github.com/adi1090x/polybar-themes#-polybar-12).

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
