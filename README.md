# Script de descarga y procesamiento de vídeos de YouTube

Este repositorio contiene un script bash que permite descargar un vídeo de YouTube, extraer su audio en formato MP3 y generar un vídeo comprimido sin audio. 
El script verifica si las herramientas necesarias están instaladas (`yt-dlp` y `ffmpeg`) y en caso contrario, las instala automáticamente.

## Requisitos

- Sistema operativo Linux (probado en Ubuntu 22.04)
- Conexión a internet
- Permisos de usuario con capacidad de usar `sudo` para instalar paquetes

## Herramientas usadas

- [yt-dlp](https://github.com/yt-dlp/yt-dlp): herramienta para descargar vídeos y audios desde plataformas como YouTube.
- [ffmpeg](https://ffmpeg.org/): biblioteca para procesamiento de audio y vídeo.

## Descripción del script

El script realiza las siguientes acciones:

1. Comprueba si `yt-dlp` y `ffmpeg` están instalados; si no, los instala automáticamente.
2. Solicita al usuario la URL de un vídeo de YouTube.
3. Muestra los formatos de vídeo disponibles para esa URL.
4. Permite seleccionar el formato deseado.
5. Descarga el vídeo en el formato seleccionado.
6. Extrae el audio en formato MP3 del vídeo descargado.
7. Genera un vídeo sin audio comprimido con el códec H.265.
8. Muestra información técnica del audio y del vídeo resultantes.
