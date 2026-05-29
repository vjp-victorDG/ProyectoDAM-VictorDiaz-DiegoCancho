# Configuración de Balanceador de Carga (Nginx)

## 1. Bloque Upstream
En el archivo `/etc/nginx/nginx.conf`, definimos los servidores web:
```nginx
upstream mi_proyecto {
    server 192.168.1.10; # Servidor Web 01
    server 192.168.1.11; # Servidor Web 02
}

server {
    listen 80;
    location / {
        proxy_pass http://mi_proyecto;
    }
}