# Valdaryon — actualizaciones

Este repositorio lo usa el **lanzador de Valdaryon** para actualizar el juego. Aquí solo está el juego armado de cada versión,
su número de versión y su firma. No hay código del servidor, herramientas ni documentos.

- `version.json`: la versión publicada (firmada). Es lo primero que lee el lanzador.
- `manifiesto.json`: la lista de archivos de la versión con su SHA-256 (firmada con ed25519).
- `archivos/ab/<sha256>`: cada archivo del juego, guardado por su SHA-256.
- `noticias.json` y `estado.json`: noticias y mantenimiento del lanzador (firmados).

Cada versión es una Release con la etiqueta `vX.Y.Z`. El lanzador rechaza todo lo que no esté firmado con la clave oficial.
