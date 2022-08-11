# Instalar-impresora-epson-en-kali
```
sudo apt-get install cups cups-client
```
```
sudo adduser root lpadmin
```
```
sudo nano /etc/group
```
En el archivo filtra por **lpadmin** y remplasa la linea **lpadmin:x:158:root** por:
```
lpadmin:x:158:root,<user>
```
Guarda y cierra el archivo
```
sudo apt install printer-driver-escpr
```
```
/etc/init.d/cups start
```
```
reboot
```
En el navegador ve a [Cups](https://localhost:631/admin/) y añade tu impresora con el driver indicado

