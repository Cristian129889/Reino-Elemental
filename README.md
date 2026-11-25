# Reino Elemental — actualizaciones

Este repositorio publica los archivos que el cliente descarga desde GitHub.

## Archivos

- `version.txt`: versión del cliente (`version:5.18`). El cliente quita el prefijo y los saltos de línea antes de comparar.
- `version_som.txt`, `version_maps.txt`: versiones de sonidos y mapas.
- `reino.zip`: paquete compilado del cliente. El actualizador lo descomprime en `download` y lo copia sobre el juego.
- `actualizador.zip`: ayudante que aplica el paquete.
- `msgSpanish.txt`, `msgEnglish.txt`, `msgPortuguese.txt`, `msgFrench.txt`: mensaje del día (MOTD). También hay copias en minúsculas para coincidir con `msg<idiomajogo>.txt`.
- `lang/index.txt`: lista de traducciones disponibles, una por línea.
- `lang/*.lang`: traducciones que se pueden descargar o borrar desde el menú de administración → traducciones.

## Cómo actualizar

Edita el archivo correspondiente y haz commit/push en `main`. El cliente lee las URLs `raw.githubusercontent.com/Cristian129889/Reino-Elemental/main/...` definidas en `config-test.nvgt`.
