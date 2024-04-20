# Diccionario de Comandos y Trucos para Ubuntu

## Comandos Básicos de Terminal

### Navegación de Directorios
- `cd`: Cambiar de directorio.
- `ls`: Listar contenido de un directorio.
- `pwd`: Mostrar el directorio actual.

### Manipulación de Archivos y Directorios
- `mkdir nombre_directorio`: Crear un nuevo directorio.
- `touch nombre_archivo`: Crear un nuevo archivo vacío.
- `cp archivo_origen archivo_destino`: Copiar un archivo.
- `mv archivo_origen archivo_destino`: Mover o renombrar un archivo.
- `rm archivo`: Eliminar un archivo.
- `rmdir directorio`: Eliminar un directorio vacío.

## Atajos de Teclado
- `Ctrl + Alt + T`: Abrir terminal.
- `Ctrl + C`: Cancelar la ejecución de un comando.
- `Ctrl + D`: Cerrar la terminal actual.

## Gestión de Paquetes
- `sudo apt update`: Actualizar la lista de paquetes.
- `sudo apt upgrade`: Actualizar todos los paquetes instalados.
- `sudo apt install nombre_paquete`: Instalar un nuevo paquete.
- `sudo apt remove nombre_paquete`: Desinstalar un paquete.

## Personalización del Entorno
- `sudo apt install gnome-tweaks`: Instalar GNOME Tweaks para personalización.
- `gnome-tweaks`: Abrir GNOME Tweaks para personalizar el escritorio.
- `gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'`: Configurar Dash to Dock para minimizar al hacer clic.

## Redes y Conectividad
- `ifconfig`: Mostrar información de red.
- `ping direccion_ip`: Enviar paquetes ICMP a una dirección IP.
- `sudo lshw -C network`: Mostrar información detallada del hardware de red.

## Seguridad y Privacidad
- `sudo ufw enable`: Activar el Firewall.
- `sudo ufw status`: Verificar el estado del Firewall.
- `sudo ufw allow puerto`: Permitir tráfico en un puerto específico.
- `sudo ufw deny puerto`: Denegar tráfico en un puerto específico.

## Administración del Sistema
- `sudo apt autoremove`: Eliminar paquetes huérfanos.
- `sudo systemctl start nombre_servicio`: Iniciar un servicio.
- `sudo systemctl stop nombre_servicio`: Detener un servicio.
- `sudo systemctl restart nombre_servicio`: Reiniciar un servicio.