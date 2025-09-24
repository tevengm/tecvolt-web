# TecVolt — Sitio Web (GitHub Pages)

Sitio web corporativo de **TecVolt** para servicios de reparación, mantenimiento y ensamble de computadores y celulares (Bucaramanga, Colombia). Proyecto **estático**, sin frameworks, publicado en **GitHub Pages** y mapeado a dominio propio.

---

## 📁 Estructura

```
/
├─ index.html
└─ assets/
   ├─ logo.png
   ├─ hero-bg@mobile.jpg
   ├─ hero-bg@desktop.jpg
   ├─ og-cover.jpg
   ├─ favicon-16.png
   ├─ favicon-32.png
   └─ apple-touch-icon.png
```

---

## ✨ Características

- **UI limpia** con paleta oscura y acento cian.
- **Header fijo** y **menú móvil** accesible.
- **Hero** con 1 imagen (overlay para legibilidad).
- Secciones: **Servicios**, **Trabajos (YouTube)**, **FAQ**, **Contacto**.
- Botón **WhatsApp** flotante.
- Metadatos **Open Graph** (compartir en redes).
- **Favicon** y **apple-touch-icon** listos.
- Snippet **JSON-LD LocalBusiness** para SEO local.

---

## 🚀 Publicación (GitHub Pages)

1. Sube el repo con `index.html` en la raíz.
2. En **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: `main` / `/ (root)`.
3. Espera el build. La URL será `https://<usuario>.github.io/<repo>/`.

### Dominio propio (Namecheap)
1. En el repo, crea el archivo `CNAME` (en la raíz) con:
   ```
   tecvolt.net
   ```
2. En **Namecheap → Domain List → Advanced DNS**:
   - **Tipo A (@)** → IP de GitHub Pages:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - **CNAME (www)** → `<usuario>.github.io.`
3. Espera propagación DNS y prueba `https://tecvolt.net/`.

> **Correo**: para recibir en Gmail sin pagar, usa **Email Forwarding** en Namecheap → `info@tecvolt.net` → tu Gmail.

---

## 🖼️ Assets e imágenes

- **Hero desktop**: `assets/hero-bg@desktop.jpg` → 1920×1080 (≈200–320 KB).
- **Hero móvil**: `assets/hero-bg@mobile.jpg` → 1200×800 (≈150–220 KB).
- **Open Graph**: `assets/og-cover.jpg` → **1200×630**.
- **Favicons**:
  - `favicon-16.png` → 16×16
  - `favicon-32.png` → 32×32
  - `apple-touch-icon.png` → 180×180  
- **Logo**: `assets/logo.png` (mejor si también tienes `.svg`).

> Tip: comprime con [TinyPNG](https://tinypng.com) o [Squoosh](https://squoosh.app) antes de subir.

---

## ⚙️ Personalización rápida

- Cambia textos y enlaces de WhatsApp/Instagram/YouTube en `index.html`.
- Sustituye **hero**: reemplaza `hero-bg@*.jpg`.
- Ajusta paleta en `:root` dentro del `<style>`:
  ```css
  --accent:#0aa3e0; --bg:#07101a; --card:#0f1720; --text:#e6eef6; --muted:#9fb6c6;
  ```
- Para compartir en redes, edita metadatos en `<head>`:
  ```html
  <meta property="og:title" content="TecVolt · Reparación y Ensamble" />
  <meta property="og:description" content="Soluciones tecnológicas confiables..." />
  <meta property="og:image" content="https://tecvolt.net/assets/og-cover.jpg" />
  ```

---

## ✅ Accesibilidad & SEO

- Enlaces con `aria-label`, `role` y `id` para navegación.
- Contraste alto + overlay en hero para legibilidad.
- **JSON-LD** tipo `LocalBusiness` con `areaServed`.
- **Scroll suave** y `focus-visible` para teclado.

---

## 📱 Rendimiento

- **Preload** de la imagen hero (mejora LCP).
- Imágenes **responsivas** por media queries (mobile/desktop).
- Evita PNG para fotos; usa JPG con calidad 70–80%.
- Mantén cada imagen grande **< 320 KB**.

---

## 🔧 Solución de problemas

- **Facebook en iPhone abre en blanco**: abrir en la **misma pestaña** (sin `target="_blank"`) o usar `https://m.facebook.com/…`.
- **Cambios no se ven**: hacer hard-reload (Ctrl/Cmd+Shift+R) y revisar GitHub Pages **Actions/Build**.
- **SSL/HTTPS**: en **Settings → Pages**, activa **Enforce HTTPS** cuando esté disponible.

---

## 🧩 Créditos

- **Fuente**: [Inter](https://fonts.google.com/specimen/Inter) (Google Fonts).
- **Iconos**: [Font Awesome](https://fontawesome.com) CDN.
- **YouTube Embeds**: iframes oficiales.

---

## 📄 Licencia

Código del sitio: MIT (ajústala según necesites).  
Contenido (logos, imágenes, textos): © TecVolt.  

---

## 📬 Contacto

- WhatsApp: **+57 318 442 4423**  
- Email: **tecvoltcolombia@gmail.com**  
- Web: **https://tecvolt.net/**

---

### Checklist de publicación

- [ ] Subir `index.html` y carpeta `assets/`.
- [ ] Comprimir `hero-bg@*.jpg`.
- [ ] Poner `og-cover.jpg` (1200×630).
- [ ] Agregar `CNAME` con `tecvolt.net`.
- [ ] Configurar A/CNAME en Namecheap.
- [ ] Activar **Email Forwarding** `info@tecvolt.net` → Gmail.  
- [ ] Verificar **Enforce HTTPS** en GitHub Pages.
