# Diccionario de Comandos y Trucos para Ubuntu

## Comandos Básicos de Terminal

### Navegación de Directorios
- `cd`: Cambiar de directorio.
- `ls`: Listar contenido de un directorio.
- `pwd`: Mostrar el directorio actual.

### Visualización de Archivos
- `cat nombre_archivo`: Mostrar el contenido completo de un archivo en la terminal.
- `less nombre_archivo`: Visualizar el contenido de un archivo página por página con capacidad de desplazamiento.
- `head nombre_archivo`: Mostrar las primeras líneas de un archivo.
- `tail nombre_archivo`: Mostrar las últimas líneas de un archivo.

### Manipulación de Archivos y Directorios
- `mkdir nombre_directorio`: Crear un nuevo directorio.
- `touch nombre_archivo`: Crear un nuevo archivo vacío.
- `cp archivo_origen archivo_destino`: Copiar un archivo.
- `mv archivo_origen archivo_destino`: Mover o renombrar un archivo.
- `rm archivo`: Eliminar un archivo.
- `rmdir directorio`: Eliminar un directorio vacío.
- `chmod permisos nombre_archivo`: Cambiar los permisos de un archivo o directorio.
- `chown nuevo_propietario nombre_archivo`: Cambiar el propietario de un archivo o directorio.
- `find directorio -name nombre_archivo`: Buscar un archivo en un directorio específico.

## Atajos de Teclado
- `Ctrl + Alt + T`: Abrir terminal.
- `Ctrl + Shift + T`: Abrir una nueva pestaña en el terminal.
- `Ctrl + L`: Limpiar la pantalla del terminal.
- `Ctrl + C`: Cancelar la ejecución de un comando.
- `Ctrl + D`: Cerrar la terminal actual.

## Gestión de Paquetes
- `sudo apt update`: Actualizar la lista de paquetes.
- `sudo apt upgrade`: Actualizar todos los paquetes instalados.
- `sudo apt install ./nombre_paquete.deb`: Instalar un nuevo paquete situado en la misma carpeta en la que nos encontremos.
- `sudo apt remove nombre_paquete`: Desinstalar un paquete.
- `apt-cache search término`: Buscar paquetes relacionados con un término específico.
- `apt-get remove --purge nombre_paquete`: Eliminar un paquete y sus archivos de configuración.

## Personalización del Entorno
- `sudo apt install gnome-tweaks`: Instalar GNOME Tweaks para personalización.
- `gnome-tweaks`: Abrir GNOME Tweaks para personalizar el escritorio.
- `gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'`: Configurar Dash to Dock para minimizar al hacer clic.
- `dconf-editor`: Editor gráfico para configuraciones avanzadas del sistema.
- `gnome-session-properties`: Administrador de sesiones para controlar los programas que se ejecutan al inicio.

## Redes y Conectividad
- `ifconfig`: Mostrar información de red.
- `ping direccion_ip`: Enviar paquetes ICMP a una dirección IP.
- `sudo lshw -C network`: Mostrar información detallada del hardware de red.
- `netstat -tuln`: Mostrar puertos de red y aplicaciones que los utilizan.
- `nmap direccion_ip`: Escanear puertos en una dirección IP para detectar servicios en ejecución.

## Seguridad y Privacidad
- `sudo ufw enable`: Activar el Firewall.
- `sudo ufw status`: Verificar el estado del Firewall.
- `sudo ufw allow puerto`: Permitir tráfico en un puerto específico.
- `sudo ufw deny puerto`: Denegar tráfico en un puerto específico.
- `gpg --gen-key`: Generar un nuevo par de claves GPG para cifrado y firmas.
- `gpg --export -a "Nombre Usuario" > clave_publica.asc`: Exportar la clave pública para compartir.
- `gpg --import clave_publica.asc`: Importar una clave pública de otro usuario.

## Administración del Sistema
- `sudo apt autoremove`: Eliminar paquetes huérfanos.
- `sudo systemctl start nombre_servicio`: Iniciar un servicio.
- `sudo systemctl stop nombre_servicio`: Detener un servicio.
- `sudo systemctl restart nombre_servicio`: Reiniciar un servicio.
- `top`: Mostrar los procesos en ejecución y su uso de recursos en tiempo real.
- `htop`: Visualizar de manera interactiva los procesos en ejecución y su uso de recursos.
