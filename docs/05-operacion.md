# Guía de Operación y Mantenimiento Diario

## 1. Checklist Diario
* [ ] Verificar que los servicios Nginx y MySQL estén activos (`systemctl status`).
* [ ] Revisar logs de errores en `/var/log/nginx/error.log`.
* [ ] Verificar espacio en disco restante: `df -h`.

## 2. Mantenimiento Preventivo
* **Semanal:** Actualización de repositorios y paquetes: `sudo apt update && sudo apt upgrade -y`.
* **Mensual:** Limpieza de logs antiguos y optimización de tablas BBDD.