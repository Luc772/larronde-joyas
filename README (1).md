# ORA — Joyas bañadas en oro

Página web de una sola pieza (`index.html`), sin dependencias de build. Lista para publicar con **GitHub Pages**.

## Cómo publicarla en GitHub

1. Crea un repositorio nuevo en GitHub (por ejemplo `joyas-ora`).
2. Sube `index.html` (y este `README.md` si quieres) al repositorio:
   - Desde la web de GitHub: botón **Add file → Upload files**, arrastra `index.html`, commit.
   - O desde tu computador:
     ```bash
     git init
     git add .
     git commit -m "Primera versión del sitio"
     git branch -M main
     git remote add origin https://github.com/TU-USUARIO/joyas-ora.git
     git push -u origin main
     ```
3. En el repositorio, ve a **Settings → Pages**.
4. En "Build and deployment", elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`. Guarda.
5. Espera 1–2 minutos. Tu sitio quedará publicado en:
   `https://TU-USUARIO.github.io/joyas-ora/`

## Estructura de archivos

```
index.html
img/
  clasico.jpg
  paperclip.jpg
  colaraton.jpg
  ovalado.jpg
```

Sube la carpeta `img/` junto con `index.html` — el catálogo carga las fotos desde ahí (`<img src="img/clasico.jpg">`). Si subes por la web de GitHub, arrastra la carpeta completa en **Add file → Upload files**.

## Qué personalizar antes de publicar

- **WhatsApp**: reemplaza `56966504587` en los 3 enlaces `wa.me` por tu número real (código de país + número, sin espacios ni +).
- **Instagram**: reemplaza el enlace `https://instagram.com` por tu cuenta.
- **Productos**: cada tarjeta en la sección "Catálogo" tiene nombre, descripción, precio y specs — edítalos directo en el HTML (busca `<div class="name">`).
- **Fotos reales**: los productos usan íconos dibujados en SVG como marcador visual. Cuando tengas fotos, reemplaza el `<svg>...</svg>` dentro de cada `.card-img` por `<img src="fotos/producto1.jpg" alt="Collar Vela">`.
- **Nombre de marca**: reemplaza "ORA" en el logo (`<a class="logo">`) por el nombre real de tu tienda.

## Estructura del diseño

- Fondo oscuro cálido con acento dorado, tipografía serif (Fraunces) + sans (Work Sans) + mono (Space Mono) para specs técnicas.
- Elemento distintivo: diagrama de "capas de oro" en el hero, que refleja el proceso real de baño en oro (base de acero, barrera sin níquel, capa de oro en micras).
- Totalmente responsive (celular, tablet, escritorio) y con botón flotante de WhatsApp.
