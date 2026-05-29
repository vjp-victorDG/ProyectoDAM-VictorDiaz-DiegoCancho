# Backups (Copias de Seguridad)

## 1. Política de Copias
* **Frecuencia:** [Ej: Diaria]
* **Tipo:** [Ej: Incremental]
* **Destino:** [Ej: Servidor remoto / Nube / Disco externo]

## 2. Scripts y Automatización
* **Script de backup:** `/scripts/backup.sh`
* **Programación (Cron):** `0 2 * * * /scripts/backup.sh`

## 3. Procedimiento de Restauración
1. Ubicar el archivo comprimido `.tar.gz`.
2. Extraer en la ruta destino: `tar -xzvf backup_fecha.tar.gz -C /ruta/destino`