# Base de Datos

## 1. Configuración del Sistema
* **Motor de BBDD:** [Ej: MySQL, MariaDB, PostgreSQL]
* **Versión:** [Ej: 8.0, 10.6, 14.x]
* **Puerto:** [Ej: 3306, 5432]

CAMBIO

## 2. Configuración Inicial
1. Instalación: `sudo apt install [nombre-paquete]`
2. Asegurar instalación: `sudo mysql_secure_installation`
3. Creación de usuario y base de datos:
   - `CREATE DATABASE nombre_db;`
   - `CREATE USER 'usuario'@'localhost' IDENTIFIED BY 'password';`
   - `GRANT ALL PRIVILEGES ON nombre_db.* TO 'usuario'@'localhost';`

## 3. Mantenimiento
* **Ruta de logs:** `/var/log/mysql/error.log`
* **Comando de reinicio:** `sudo systemctl restart [nombre-servicio]`

## 4. Estructura de tablas
* [Tabla 1]: [Breve descripción de los campos]
* [Tabla 2]: [Breve descripción de los campos]