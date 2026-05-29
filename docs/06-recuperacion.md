# Plan de Recuperación (DRP)

## 1. Procedimiento ante caída del Servidor Web
1. Intentar reinicio suave: `sudo systemctl reload nginx`.
2. Si persiste: Verificar sintaxis de configuración con `nginx -t`.
3. Si el error es crítico: Desplegar configuración desde el último backup.

## 2. Procedimiento ante fallo de Base de Datos
1. Verificar si el proceso MySQL está activo.
2. Si la BBDD está corrupta:
   * Detener servicio.
   * Importar desde el último dump de seguridad (`mysql -u usuario -p base_datos < backup.sql`).
   * Verificar integridad con `CHECK TABLE`.