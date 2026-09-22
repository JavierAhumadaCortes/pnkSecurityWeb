# Ejecucion local de pnkSecurity con Docker Compose

Esta configuracion levanta tres contenedores:

- `web`: Apache con PHP 7.4 y extensiones MySQL.
- `db`: MySQL 8.0 con importacion automatica de `Script_BD/pnk_security.sql`.
- `phpmyadmin`: interfaz local para revisar la base de datos.

> PHP 7.4 se usa para aumentar la compatibilidad con este proyecto antiguo. Esta
> version ya no recibe actualizaciones de seguridad. Utiliza este entorno solo
> como laboratorio local y no lo publiques directamente en Internet.

## 1. Ubicar los archivos

Copia el contenido de este paquete en la raiz del proyecto, donde estan
`index.php`, `carrito.php`, la carpeta `Script_BD` y las demas carpetas:

```text
pnkSecurity/
|-- compose.yaml
|-- Dockerfile
|-- index.php
|-- carrito.php
|-- Script_BD/
|   `-- pnk_security.sql


