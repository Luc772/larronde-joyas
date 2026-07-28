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
```

Todo el sitio (incluidas las fotos de los productos) está en un solo archivo `index.html`. Las imágenes van incrustadas dentro del código, así que basta con subir ese archivo — no necesitas una carpeta `img/` aparte.

## Qué personalizar antes de publicar

- **WhatsApp**: reemplaza `56966504587` en los 3 enlaces `wa.me` por tu número real (código de país + número, sin espacios ni +).
- **Instagram**: reemplaza el enlace `https://instagram.com` por tu cuenta.
- **Productos**: cada tarjeta en la sección "Catálogo" tiene nombre, descripción, precio y specs — edítalos directo en el HTML (busca `<div class="name">`).
- **Fotos**: las imágenes están incrustadas en base64 dentro del HTML. Si quieres cambiar alguna, busca en el código el bloque `<img src="data:image/jpeg;base64,...">` correspondiente al producto y reemplaza esa línea completa, o pide ayuda para hacerlo con una foto nueva.
- **Nombre de marca**: reemplaza "ORA" en el logo (`<a class="logo">`) por el nombre real de tu tienda.

## Estructura del diseño

- Fondo oscuro cálido con acento dorado, tipografía serif (Fraunces) + sans (Work Sans) + mono (Space Mono) para specs técnicas.
- Elemento distintivo: diagrama de "capas de oro" en el hero, que refleja el proceso real de baño en oro (base de acero, barrera sin níquel, capa de oro en micras).
- Totalmente responsive (celular, tablet, escritorio) y con botón flotante de WhatsApp.
