sudo apt update

sudo apt install build-essential -y

#### Instalar terminator
```
sudo apt-get install terminator
```


#### Configurar layout de teclado

##### No Ubuntu 19.10 - configurar teclado internacional
 - Configurações > Região e idioma
  - Adicionar o idioma: Inglês (EUA,intern. alt.)
  - Alterar o arquivo: /etc/environment
     - Adicionar:
     ```
     GTK_IM_MODULE=cedilla
     QT_IM_MODULE=cedilla
     ```

#### Font FiraCode
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
```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
```

#### Problema com endereço local
```
https://askubuntu.com/questions/81797/nslookup-finds-ip-but-ping-doesnt
```
