# Reporte Móvil — PWA

App móvil (Visión · Familias · Stock · Tallas/Colores) para las 6 tiendas, en un solo archivo.

## Contenido
- `index.html`  — la app (con los datos incrustados).
- `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png` — piezas de la PWA.

## Publicar en GitHub Pages
1. Crear un repo (ej. `reporte-tiendas`) y subir estos 5 archivos a la raíz.
2. Settings → Pages → Branch: `main` / carpeta `/root` → Save.
3. Abrir la URL `https://<usuario>.github.io/reporte-tiendas/` en el celular.
4. Chrome → menú (⋮) → **Agregar a pantalla de inicio**. Queda como una app con ícono.

## Actualizar (1 vez al mes)
1. Regenerar: `python3 gen_mobile_drill.py` (usa los dashboards ya actualizados).
2. Copiar el nuevo `pwa_movil/index.html` al repo y `git push`.
   (El generador ya sube la VERSION del `sw.js`, así la PWA se refresca sola al abrirla online.)
