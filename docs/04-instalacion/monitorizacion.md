# Monitorización

## 1. Herramientas de Monitorización
* **Herramienta:** [Ej: Prometheus, Grafana, Zabbix o Netdata]
* **Objetivo:** Supervisar el uso de CPU, RAM, espacio en disco y estado de servicios.

## 2. Métricas clave
* **CPU:** Alerta si supera el [80]% de uso sostenido.
* **Memoria RAM:** Alerta si supera el [85]% de uso.
* **Disco:** Alerta si el espacio libre es inferior a [10] GB.

## 3. Logs del sistema
* **Ubicación logs principales:** `/var/log/syslog`
* **Herramienta de visualización:** `journalctl`