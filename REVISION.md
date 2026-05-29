# REVISION.md - Reflexión del Proyecto

## 1. Gestión de Conflictos
Durante el desarrollo surgieron conflictos al intentar hacer el *merge* de ramas que modificaban archivos comunes simultáneamente.
* **Resolución:** Adoptamos la política de realizar `git pull origin main` frecuentemente en nuestras ramas locales para integrar los cambios del compañero antes de subir los nuestros. Cuando surgieron conflictos de escritura, los resolvimos comparando línea a línea en el editor y seleccionando la versión correcta antes de completar el `commit`.

## 2. Comandos Git más utilizados
Nuestra rutina diaria se basó en el uso de los siguientes comandos (o sus equivalentes en la interfaz gráfica):
* `git checkout -b [nombre-rama]`: Para crear los entornos de trabajo aislados.
* `git add .` / `git commit -m "..."`: Para registrar los cambios de forma incremental.
* `git push origin [nombre-rama]`: Para subir el trabajo al repositorio remoto.
* `git pull origin main`: Para mantener la rama local actualizada.
* `git merge`: Utilizado principalmente a través de *Pull Requests* para integrar cambios a la rama principal.

## 3. ¿Qué haríamos diferente en un próximo proyecto?
* **Planificación inicial:** Dedicaríamos más tiempo a definir el esquema de directorios y los nombres de los archivos antes de empezar a programar para evitar solapamientos.
* **Comentarios:** Estableceríamos una comunicación más activa en los *Pull Requests* durante la fase temprana de desarrollo para asegurar que ambos entendemos la configuración de infraestructura del otro.
* **Automatización:** Implementaríamos un pequeño *script* de despliegue para probar la configuración de Nginx automáticamente al recibir un nuevo *commit*.

## 4. Reflexión sobre el intercambio de roles
El intercambio de roles resultó ser una decisión muy acertada:
* **Ventajas:** Nos permitió comprender los problemas que el otro enfrentaba, evitando la creación de "islas de conocimiento". El documentalista de operaciones pudo dar *feedback* técnico al de plataforma sobre cómo hacer las configuraciones más "mantenibles".
* **Resultado:** La rotación nos forzó a leer y entender el código del compañero en profundidad, lo que mejoró significativamente la calidad final de la documentación y redujo los errores en la configuración del balanceador de carga.