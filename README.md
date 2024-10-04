# Comandos y Scripts
Repositorio de scripts y comandos en bash

**Comandos**

Borrar imágenes thumbnails de archivos personales.
```
sudo rm -rf ~/.cache/thumbnails/*
```
Borra archivos de configuración de paquetes desinstalados.
```
sudo apt purge $(dpkg -l | awk '/^rc/ { print $2 }')
```
