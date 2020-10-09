## feriados
Python script for [polybar](https://github.com/polybar/polybar) that shows next holiday in Argentina.

![](screenshot.png)

### My polybar
![](polybar.png)


Theme from [polybar-themes](https://github.com/adi1090x/polybar-themes#-polybar-12).

### Install
Add custom script module in polybar config.

```
[module/feriados]
type = custom/script  -c 00ff00 -l Próximo feriado
exec = ~/.scripts/feriados
interval = 43200   # update each 12 hours
```

### Options
```
usage: feriados [-h] [-c COLOR] [-l LABEL]

optional arguments:
  -h, --help            show this help message and exit
  -c COLOR, --color COLOR
                        Text color (default=ffab04)
  -l LABEL, --label LABEL
                        Label text (default=Feriado)
```