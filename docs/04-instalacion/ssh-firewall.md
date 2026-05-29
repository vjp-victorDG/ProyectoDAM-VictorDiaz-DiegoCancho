# SSH y Firewall

## 1. Configuración SSH
* **Puerto personalizado:** [Ej: 2222 (Recomendado cambiar el 22 por defecto)]
* **Restricción de acceso:** 
    * Permitir acceso solo por clave SSH: `PasswordAuthentication no`
    * Deshabilitar acceso root: `PermitRootLogin no`
* **Archivo de configuración:** `/etc/ssh/sshd_config`

## 2. Configuración del Firewall (UFW)
* **Estado:** `sudo ufw status`
* **Reglas aplicadas:**
    * Permitir tráfico SSH: `sudo ufw allow [tu-puerto-ssh]/tcp`
    * Permitir tráfico Web: `sudo ufw allow 'Nginx Full'` o `sudo ufw allow 80/tcp`
    * Activar firewall: `sudo ufw enable`

## 3. Seguridad Adicional
* **Monitorización de intentos de acceso:** `sudo tail -f /var/log/auth.log`
* **Herramienta sugerida:** Fail2Ban (para banear IPs con intentos fallidos de conexión).

## Configuración de firewall con UFW
- `ufw default deny incoming`
- `ufw allow 22/tcp`   # SSH para administración
- `ufw allow 80,443/tcp`  # Web
- `ufw enable`