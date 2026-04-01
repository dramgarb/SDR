# Scripts de Automatizacion - Practica 2º Trimestre ASIR

Este repositorio contiene las herramientas necesarias para la gestion automatizada de un servidor de hosting en AWS.

## Script para la automatizacion del proceso de hosting: creacion de usuario, carpetas, virtual host, registros DNS y base de datos SQL

Este script (master_hosting.sh) realiza todas las tareas necesarias para dar de alta a un nuevo cliente en el servidor de forma automatica.

#!/bin/bash
USER=$1
IP_PRIVADA="172.31.25.176"
DOMAIN="marisma.intranet"
PASS="Hosting2026!"

if [ $# -ne 1 ]; then
    echo "Uso: $0 <nombre_usuario>"
    exit 1
fi

# Creacion de usuario del sistema y directorio web
sudo useradd -m -s /bin/bash $USER
echo "$USER:$PASS" | sudo chpasswd
sudo mkdir -p /var/www/html/$USER
echo "<h1>Web de $USER</h1>" | sudo tee /var/www/html/$USER/index.html
sudo chown -R $USER:$USER /var/www/html/$USER

# Configuracion de Virtual Host en Apache
CONF="/etc/apache2/sites-available/$USER.conf"
sudo bash -c "cat > $CONF" <<EOF
<VirtualHost *:80>
    ServerName $USER.$DOMAIN
    DocumentRoot /var/www/html/$USER
</VirtualHost>
EOF
sudo a2ensite $USER.conf

# Actualizacion de DNS (Resolucion directa e inversa)
echo "$USER  IN  A  $IP_PRIVADA" | sudo tee -a /etc/bind/db.marisma.intranet
echo "176  IN  PTR  $USER.$DOMAIN." | sudo tee -a /etc/bind/db.172.31.25

# Creacion de base de datos y privilegios SQL
sudo mariadb -u root -e "CREATE DATABASE db_$USER; GRANT ALL PRIVILEGES ON db_$USER.* TO '$USER'@'localhost' IDENTIFIED BY '$PASS'; FLUSH PRIVILEGES;"

# Reinicio de servicios para aplicar cambios
sudo systemctl reload apache2 bind9
echo "FINALIZADO: Accede a http://$USER.$DOMAIN"

---

## Script de prueba para verificar la ejecucion de Python en el servidor web mediante CGI

Este script (prueba.py) permite comprobar que el servidor Apache esta configurado correctamente para ejecutar aplicaciones Python.

#!/usr/bin/python3
print("Content-type: text/html\n\n")
print("<h1>Python funcionando en el Servidor de Hosting</h1>")
print("<p>Practica de 2º Trimestre - ASIR</p>")

---

## Instrucciones de uso
1. Dar permisos de ejecucion: chmod +x nombre_del_script.sh
2. Ejecutar con privilegios de superusuario: sudo ./nombre_del_script.sh
