# Reino Elemental — actualizaciones

Este repositorio publica los archivos que el cliente descarga desde GitHub.

## Archivos

- `version.txt`: versión del cliente (`version:5.34`). El cliente quita el prefijo y los saltos de línea antes de comparar.
- `Reino Elemental.exe`: ejecutable del cliente. Se descarga solo este archivo y `actualizador.exe` lo reemplaza cuando el juego ya se cerró.
- `version_som.txt`, `version_maps.txt`: versiones de sonidos y mapas.
- `sounds/index.txt`: sonidos `.ogg` publicados, uno por línea como `nombre.ogg|sounds/nombre%20codificado.ogg`. El cliente compara con su carpeta `sounds` y solo baja los `.ogg` que faltan; si no falta ninguno, anota la versión sin descargar ni reiniciar. Incluye `notify_message.ogg`, el aviso del mensaje del día.
- `maps.map`: paquete único con los 526 mapas cifrados con `MAPS_ENCRYPTION_KEY`. El cliente descarga solo este archivo; ya no pide `.map` sueltos.
- `maps/index.txt`: se mantiene solo como referencia de los mapas publicados; el actualizador ya no lo usa.
- `reino.zip`: paquete compilado completo, se mantiene como copia de seguridad; la actualización normal ya no lo usa.
- `actualizador.zip`: ayudante que aplica el paquete.
- `msgSpanish.txt`, `msgEnglish.txt`, `msgPortuguese.txt`, `msgFrench.txt`: mensaje del día (MOTD). También hay copias en minúsculas para coincidir con `msg<idiomajogo>.txt`.
- `lang/index.txt`: lista de traducciones disponibles, una por línea.
- `lang/*.lang`: traducciones que se pueden descargar o borrar desde el menú de administración → traducciones.

## Cómo actualizar

Edita el archivo correspondiente y haz commit/push en `main`. El cliente lee las URLs `raw.githubusercontent.com/Cristian129889/Reino-Elemental/main/...` definidas en `config-test.nvgt`.
