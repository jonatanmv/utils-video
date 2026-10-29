# utils-video

## Reempaquetar
cd /ruta/de/tu/carpeta
for f in *.[mM][tT][sS]; do [ -f "$f" ] && ffmpeg -i "$f" -c:v copy -c:a aac "${f%.*}.mp4"; done
