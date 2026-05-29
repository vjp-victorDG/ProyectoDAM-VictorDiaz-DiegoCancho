# Servidor Web - Configuración Técnica

## 1. Stack Tecnológico
* **Servidor:** Nginx (Recomendado por su alto rendimiento).
* **Entorno:** Ubuntu 22.04 LTS.

## 2. Configuración del Virtual Host
* **Ruta de configuración:** `/etc/nginx/sites-available/proyecto`
* **Directiva clave:** `listen 80; server_name midominio.com;`

## 3. Optimización y Seguridad
* **SSL/TLS:** Configurado mediante Let's Encrypt (Certbot).
* **Compresión:** Gzip activado para reducir tiempos de carga.