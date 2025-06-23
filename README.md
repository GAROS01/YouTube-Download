# Descargador de Videos de YouTube

Un script simple en Python para descargar videos de YouTube usando `yt-dlp`.

## Descripción

Este script permite descargar videos de YouTube en formato MP4 con la mejor calidad disponible. Utiliza la biblioteca `yt-dlp`, que es un fork mejorado de `youtube-dl`.

## Versión Completa

🔗 **Para una versión más completa y con más características, visita el repositorio oficial:**  
**https://github.com/GAROS01/youtube-downloader**

Esta versión incluye características adicionales como interfaz gráfica, múltiples formatos, descarga de playlists y más opciones de configuración.

## Requisitos

- Python 3.6 o superior
- Biblioteca `yt-dlp`

## Instalación

1. Instala Python si no lo tienes instalado
2. Instala la dependencia requerida:

```bash
pip install yt-dlp
```

## Uso

1. Abre el archivo [`script.py`](script.py)
2. Reemplaza la variable `url` con el enlace del video de YouTube que deseas descargar:
   ```python
   url = "https://www.youtube.com/watch?v=VIDEO_ID"
   ```
3. Ejecuta el script:
   ```bash
   python script.py
   ```

## Características

- Descarga videos en formato MP4 por defecto
- Selecciona automáticamente la mejor calidad disponible
- Combina video y audio para obtener el mejor resultado
- Manejo de errores integrado
- Nombres de archivo basados en el título del video

## Personalización

Puedes modificar el formato de descarga cambiando el parámetro `formato` en la función [`descargar_video`](script.py):

```python
descargar_video(url, formato="webm")  # Para formato WebM
```

## Estructura del Proyecto

```
descarga/
├── README.md          # Este archivo
└── script.py          # Script principal de descarga
```

## Notas Importantes

- Asegúrate de tener suficiente espacio en disco para los videos descargados
- Respeta los términos de servicio de YouTube
- Los videos se guardarán en el mismo directorio donde ejecutes el script

## Solución de Problemas

Si encuentras errores durante la descarga:

1. Verifica que la URL sea válida y el video esté disponible
2. Actualiza `yt-dlp` a la última versión: `pip install --upgrade yt-dlp`
3. Revisa tu conexión a internet

## Licencia

Este proyecto es de uso libre para propósitos educativos y personales.
