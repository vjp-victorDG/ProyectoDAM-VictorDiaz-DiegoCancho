# 02 - Diseño del Sistema (Arquitectura con Balanceador)

## 1. Arquitectura de Alta Disponibilidad
* **Componentes:**
    * **Balanceador de carga:** Nginx (Recibe peticiones y distribuye el tráfico).
    * **Nodos Web (Backend):** Servidor Web 01 y Servidor Web 02 (Almacenan la aplicación).
    * **Base de datos:** Servidor dedicado de BBDD.

## 2. Flujo de tráfico
1. El usuario accede a la IP pública del Balanceador.
2. El balanceador reparte la carga entre el Servidor Web 01 y 02 mediante el algoritmo "Round Robin".