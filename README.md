# Reproductor MP3 Open Source para Google Sites

Reproductor web sin dependencias externas. Licencia MIT. Incluye portada personalizable, carga de carpeta/archivos, búsqueda, lista de reproducción, reproducción aleatoria, repetición de lista, volumen, silencio, velocidad, avance/retroceso, progreso y diseño adaptable.

## Probar localmente
Abre `index.html` en Chrome o Edge. Usa **Cargar carpeta** para elegir la carpeta que contiene tus MP3. La lectura de carpetas depende del navegador.

## Integrarlo en Google Sites
Para una experiencia fiable, aloja esta carpeta en un servicio estático HTTPS, por ejemplo GitHub Pages:
1. Crea un repositorio público en GitHub y sube `index.html`, `README.md` y `LICENSE`.
2. En Settings → Pages, publica la rama principal desde la raíz.
3. Copia la URL pública generada.
4. En Google Sites, selecciona Insertar → Incorporar → URL e introduce la URL de GitHub Pages. Ajusta el alto del marco.

Google Sites puede limitar JavaScript en el bloque de código incrustado; alojar la página por separado y embeber su URL suele ser más fiable.

## Sobre la carga automática de carpetas
Por seguridad, una página web no puede explorar por sí sola el disco duro ni mantener acceso permanente a una carpeta local. El botón **Cargar carpeta** pide al usuario seleccionar la carpeta cada vez que se inicia o se desea actualizar la biblioteca. Los archivos elegidos se leen en el navegador y no se suben a un servidor. Si necesitas que la biblioteca se actualice sola para todos los visitantes, aloja los MP3 en un servidor/almacenamiento web y publica un catálogo JSON con sus URL públicas; este prototipo no implementa ese catálogo remoto.

## Portada
Pulsa **Cambiar portada** para seleccionar una imagen. La portada seleccionada dura mientras la página siga abierta; no se sube ni se guarda en el servidor.

## Licencia
MIT. Consulta `LICENSE`.
