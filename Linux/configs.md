sudo apt update

sudo apt install build-essential -y

#### Instalar terminator
```
sudo apt-get install terminator
```


#### Configurar layout de teclado

Para funcionar acentos e ç no teclado internacional
```
setxkbmap -model abnt -layout us -variant intl
```

Para utilizar o teclado abnt2
```
setxkbmap -model abnt2 -layout br -variant abnt2
```

#### Font Frida Code
``` 
mkdir -p ~/.local/share/fonts
```
```
for type in Bold Light Medium Regular Retina; do wget -O ~/.local/share/fonts/FiraCode-$type.ttf "https://github.com/tonsky/FiraCode/blob/master/distr/ttf/FiraCode-$type.ttf?raw=true"; done
```
``` 
fc-cache -f
```

#### Instalar NVM
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
