# tecno
Guías de las clases
# 1. Entrar al modo de escritura persistente
sudo overlayroot-chroot bash -c '
# 2. Reparar instalaciones previas
dpkg --configure -a
# 3. Actualizar lista de paquetes
apt-get update
# 4. ACTUALIZAR CHROME (Prioridad Gmail)
apt-get install --only-upgrade -y google-chrome-stable
# 5. Actualizar el resto del sistema
apt-get upgrade -y -o Dpkg::Options::="--force-confold"
# 6. Salir
exit
'
# 7. Reiniciar para aplicar cambios
sudo reboot

P<%BMGBLm9KB9jQ>1
