# 🔥 Tinta en Llamas — Colectivo Literario

Sitio web estático para GitHub Pages.

## Cómo funciona

- `index.html` — Página principal (funciona con doble clic O en servidor)
- `admin.html` — Panel para agregar cuentos, imágenes y libros
- `data/` — Archivos JSON con el contenido
- `img/` — Carpeta para imágenes locales

## Subir a GitHub Pages

```bash
git init
git add .
git commit -m "Sitio inicial"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/tinta-en-llamas.git
git push -u origin main
```

Luego en GitHub: Settings → Pages → Branch: main → Save.

## Gestionar contenido

1. Abre `admin.html` (doble clic o desde el sitio)
2. Agrega cuentos / imágenes / libros
3. Pestaña Exportar → Descarga los JSON
4. Reemplaza archivos en `data/`
5. `git add . && git commit -m "Actualizar" && git push`
