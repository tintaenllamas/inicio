# 🔥 Tinta en Llamas — Colectivo Literario

Sitio web estático para GitHub Pages con panel de administración local.

## Estructura del proyecto

```
tinta-en-llamas/
├── index.html          ← Página principal (pública)
├── admin.html          ← Panel de administración
├── css/
│   ├── style.css       ← Estilos principales
│   └── admin.css       ← Estilos del panel
├── js/
│   ├── app.js          ← Lógica del sitio público
│   └── admin.js        ← Lógica del panel admin
├── data/
│   ├── cuentos.json    ← Datos de cuentos
│   ├── galeria.json    ← Datos de galería
│   └── libros.json     ← Datos de libros
└── img/                ← Carpeta para imágenes locales
```

## Cómo subir a GitHub Pages

1. **Crear repositorio en GitHub:**
   - Ve a github.com → New repository
   - Nombre: `tinta-en-llamas` (o el que prefieras)
   - Público
   - NO marques "Add a README" (ya tienes uno)

2. **Subir los archivos:**
   ```bash
   cd tinta-en-llamas
   git init
   git add .
   git commit -m "Sitio inicial de Tinta en Llamas"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/tinta-en-llamas.git
   git push -u origin main
   ```

3. **Activar GitHub Pages:**
   - En el repositorio → Settings → Pages
   - Source: "Deploy from a branch"
   - Branch: `main` / `/ (root)`
   - Save
   - En unos minutos tu sitio estará en: `https://TU_USUARIO.github.io/tinta-en-llamas/`

## Cómo gestionar contenido

### Flujo de trabajo:

1. Abre `admin.html` en tu navegador (puedes abrirlo localmente, no necesitas servidor).
2. Agrega cuentos, imágenes o libros desde las pestañas.
3. Ve a la pestaña **Exportar** y descarga los archivos JSON actualizados.
4. Reemplaza los archivos en la carpeta `data/` de tu repositorio.
5. Haz commit y push:
   ```bash
   git add data/
   git commit -m "Actualizar contenido"
   git push
   ```
6. GitHub Pages se actualiza automáticamente en 1-2 minutos.

### Imágenes:

Para la galería y portadas de libros puedes:
- **Opción A:** Subir imágenes a la carpeta `img/` del repositorio y usar rutas relativas (`img/foto.jpg`).
- **Opción B:** Usar URLs externas de imágenes ya alojadas en internet.

## Secciones del sitio

| Sección | Descripción |
|---------|-------------|
| **Inicio** | Hero con nombre del colectivo |
| **Cuentos** | Tarjetas con extracto → click para leer completo |
| **Galería** | Grid de imágenes con lightbox |
| **Libros** | Portada + sinopsis + precio + botón de compra |
| **Nosotros** | Texto del colectivo + contacto |
| **Panel** | Administración de contenido (enlace en la navegación) |

## Personalización

- **Colores:** Edita las variables CSS en `:root` dentro de `css/style.css`
- **Textos:** Edita directamente `index.html` (sección Nosotros, footer, etc.)
- **Enlace de compra:** Usa enlaces de WhatsApp, formularios de Google, o tiendas online
- **Redes sociales:** Actualiza los enlaces en la sección Nosotros de `index.html`
