# Servidor Web

## 1. Configuración del Servidor
* **Software:** [Ej: Apache, Nginx]
* **Sistema Operativo:** [Ej: Ubuntu Server 22.04 LTS]
* **Dirección IP:** [Ej: 192.168.1.XX]

## 2. Pasos de Instalación
1. Actualización del sistema: `sudo apt update && sudo apt upgrade`
2. Instalación del paquete: `sudo apt install [nombre-paquete]`
3. Configuración del puerto: [Ej: Puerto 80 para HTTP, 443 para HTTPS]

## 3. Estado del Servicio
* **Comando de verificación:** `sudo systemctl status [nombre-servicio]`
* **Archivo de configuración:** `/etc/[ruta-al-archivo-config]`

## 4. Pruebas de Funcionamiento
* **URL de acceso:** `http://localhost` o `http://[IP-servidor]`
* **Resultado esperado:** Página de bienvenida o aplicación cargando correctamente.