### Configurar layout de teclado

Para funcionar acentos e ç no teclado internacional
```
setxkbmap -model abnt -layout us -variant intl
```

Para utilizar o teclado abnt2
```
setxkbmap -model abnt2 -layout br -variant abnt2
```

### Font Frida Code
``` 
mkdir -p ~/.local/share/fonts
```
```
for type in Bold Light Medium Regular Retina; do wget -O ~/.local/share/fonts/FiraCode-$type.ttf "https://github.com/tonsky/FiraCode/blob/master/distr/ttf/FiraCode-$type.ttf?raw=true"; done
```
``` 
fc-cache -f
```
