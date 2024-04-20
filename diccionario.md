# Diccionario de Comandos y Trucos para Ubuntu

## Gestión de Usuarios

### Creación y Eliminación de Usuarios
- `sudo adduser nombre_usuario`: Crear un nuevo usuario.
- `sudo deluser nombre_usuario`: Eliminar un usuario.
- `sudo deluser --remove-home nombre_usuario`: Eliminar un usuario y su directorio de inicio.

### Cambio de Contraseña
- `sudo passwd nombre_usuario`: Cambiar la contraseña de un usuario.

### Cambio de Propietario y Permisos de Archivos
- `sudo chown nuevo_propietario archivo_o_directorio`: Cambiar el propietario de un archivo o directorio.
- `sudo chmod permisos archivo_o_directorio`: Cambiar los permisos de un archivo o directorio.

## Comandos Básicos de Terminal

### Administración de Procesos
- `ps`: Mostrar los procesos en ejecución.
- `kill PID`: Terminar un proceso utilizando su identificador de proceso (PID).
- `killall nombre_proceso`: Terminar todos los procesos con el nombre especificado.

### Navegación de Directorios
- `cd NombreDirectorio`: Cambiar de directorio.
- `cd`: Movernos al directorio home del usuario.
- `ls`: Listar contenido de un directorio.
- `pwd`: Mostrar el directorio actual.

### Visualización de Archivos
- `cat nombre_archivo`: Mostrar el contenido completo de un archivo en la terminal.
- `less nombre_archivo`: Visualizar el contenido de un archivo página por página con capacidad de desplazamiento.
- `head nombre_archivo`: Mostrar las primeras líneas de un archivo.
- `tail nombre_archivo`: Mostrar las últimas líneas de un archivo.

### Búsqueda de Archivos
- `find directorio -name nombre_archivo`: Buscar un archivo por nombre en un directorio específico.

### Comprimir y Descomprimir Archivos
- `tar -czvf archivo.tar.gz directorio`: Comprimir un directorio en un archivo .tar.gz.
- `tar -xzvf archivo.tar.gz`: Descomprimir un archivo .tar.gz.
- `zip -r archivo.zip directorio`: Comprimir un directorio en un archivo .zip.
- `unzip archivo.zip`: Descomprimir un archivo .zip.

### Manipulación de Archivos y Directorios
- `mkdir nombre_directorio`: Crear un nuevo directorio.
- `touch nombre_archivo`: Crear un nuevo archivo vacío.
- `cp archivo_origen archivo_destino`: Copiar un archivo.
- `cp -r directorio_origen directorio_destino`: Copiar un directorio y su contenido de forma recursiva.
- `mv archivo_origen archivo_destino`: Mover o renombrar un archivo.
- `rm archivo`: Eliminar un archivo.
- `rm -r directorio`: Eliminar un directorio y su contenido de forma recursiva.
- `rmdir directorio`: Eliminar un directorio vacío.
- `chmod permisos nombre_archivo`: Cambiar los permisos de un archivo o directorio.
- `chown nuevo_propietario nombre_archivo`: Cambiar el propietario de un archivo o directorio.
- `find directorio -name nombre_archivo`: Buscar un archivo en un directorio específico.

### Edición de Archivos de Texto
- `nano archivo`: Abrir un archivo para editar con el editor de texto Nano.
- `vi archivo`: Abrir un archivo para editar con el editor de texto Vi.

### Transferencia de Archivos
- `scp archivo usuario@direccion_ip:directorio_destino`: Copiar un archivo a un servidor remoto mediante SSH.
- `wget URL`: Descargar un archivo de Internet.
- `curl -O URL`: Descargar un archivo de Internet.

## Atajos de Teclado
- `Ctrl + Alt + T`: Abrir terminal.
- `Ctrl + Shift + T`: Abrir una nueva pestaña en el terminal.
- `Ctrl + L`: Limpiar la pantalla del terminal.
- `Ctrl + C`: Cancelar la ejecución de un comando.
- `Ctrl + D`: Cerrar la terminal actual.
- `Ctrl + A`: Mover el cursor al principio de la línea en el terminal.
- `Ctrl + E`: Mover el cursor al final de la línea en el terminal.

## Gestión de Paquetes
- `sudo apt update`: Actualizar la lista de paquetes.
- `sudo apt upgrade`: Actualizar todos los paquetes instalados.
- `sudo apt install ./nombre_paquete.deb`: Instalar un nuevo paquete situado en la misma carpeta en la que nos encontremos.
- `sudo apt remove nombre_paquete`: Desinstalar un paquete.
- `apt-cache search término`: Buscar paquetes relacionados con un término específico.
- `apt-get remove --purge nombre_paquete`: Eliminar un paquete y sus archivos de configuración.
- `apt-cache show nombre_paquete`: Mostrar información detallada sobre un paquete.
- `apt-get autoremove`: Eliminar paquetes huérfanos y sus dependencias.

## Personalización del Entorno
- `sudo apt install gnome-tweaks`: Instalar GNOME Tweaks para personalización.
- `gnome-tweaks`: Abrir GNOME Tweaks para personalizar el escritorio.
- `gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'`: Configurar Dash to Dock para minimizar al hacer clic.
- `dconf-editor`: Editor gráfico para configuraciones avanzadas del sistema.
- `gnome-session-properties`: Administrador de sesiones para controlar los programas que se ejecutan al inicio.
- `gsettings set org.gnome.desktop.interface gtk-theme nombre_tema`: Cambiar el tema GTK en GNOME.
- `dconf write /org/gnome/desktop/interface/cursor-theme 'nombre_tema'`: Cambiar el tema del cursor en GNOME.

## Redes y Conectividad
- `ifconfig`: Mostrar información de red. Es necesario instalar el paquete net-tools
- `ping direccion_ip`: Enviar paquetes ICMP a una dirección IP.
- `sudo lshw -C network`: Mostrar información detallada del hardware de red.
- `netstat -tuln`: Mostrar puertos de red y aplicaciones que los utilizan.
- `nmap direccion_ip`: Escanear puertos en una dirección IP para detectar servicios en ejecución.
- `nmcli`: Interfaz de línea de comandos para NetworkManager, utilizado para gestionar conexiones de red.
- `ip addr show`: Mostrar la configuración de red y direcciones IP asignadas a las interfaces de red.

## Seguridad y Privacidad
- `sudo ufw enable`: Activar el Firewall.
- `sudo ufw status`: Verificar el estado del Firewall.
- `sudo ufw allow puerto`: Permitir tráfico en un puerto específico.
- `sudo ufw deny puerto`: Denegar tráfico en un puerto específico.
- `gpg --gen-key`: Generar un nuevo par de claves GPG para cifrado y firmas.
- `gpg --export -a "Nombre Usuario" > clave_publica.asc`: Exportar la clave pública para compartir.
- `gpg --import clave_publica.asc`: Importar una clave pública de otro usuario.
- `sudo passwd usuario`: Cambiar la contraseña de un usuario.
- `ssh usuario@direccion_ip`: Iniciar una sesión SSH en un servidor remoto.

## Administración del Sistema
- `sudo systemctl start nombre_servicio`: Iniciar un servicio.
- `sudo systemctl stop nombre_servicio`: Detener un servicio.
- `sudo systemctl restart nombre_servicio`: Reiniciar un servicio.
- `top`: Mostrar los procesos en ejecución y su uso de recursos en tiempo real.
- `htop`: Visualizar de manera interactiva los procesos en ejecución y su uso de recursos.
- `sudo shutdown -h now`: Apagar el sistema inmediatamente.
- `sudo reboot`: Reiniciar el sistema.
