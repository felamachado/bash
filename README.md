# Comandos y Scripts

Borrar imágenes thumbnails de archivos personales.
```
sudo rm -rf ~/.cache/thumbnails/*
```
Borra archivos de configuración de paquetes desinstalados.
```
sudo apt purge $(dpkg -l | awk '/^rc/ { print $2 }')
```
Borra archivos de logs en /var/log/journal. Puede ser en years, months, weeks, days, hours.
```
sudo journalctl --vacuum-time=2weeks
```
