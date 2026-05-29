#### `05-operacion.md` (Operación con balanceo) 
```markdown 
# 05 - Operación en entorno balanceado 
## 1. Gestión de nodos 
* **Mantenimiento:** Para actualizar un servidor web, se debe quitar del `upstream` temporalmente para no impactar al usuario. 
* **Verificación:** `curl -I localhost` para confirmar que el balanceador responde correctamente. 
## 2. Monitorización específica * Es necesario monitorizar el balanceador (puerto 80) y cada nodo web de forma independiente para detectar si alguno se ha caído.  