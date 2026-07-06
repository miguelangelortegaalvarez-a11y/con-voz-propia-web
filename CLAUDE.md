# Con voz propia — WEB PÚBLICA

Web pública (escaparate) de **Con voz propia**, la preparación de oposiciones de Audición y Lenguaje
de **Macu** (mujer de Miguel). Es un **proyecto AUTÓNOMO e independiente**: aquí está todo lo suyo,
no depende de ninguna otra carpeta.

> La **app** (plataforma con login) es un proyecto aparte en `~/Desktop/con-voz-propia-app/`
> (repo PRIVADO). Esta web solo enlaza a ella con el botón "Acceder".

## Qué es y dónde vive

- **Repo GitHub**: `miguelangelortegaalvarez-a11y/con-voz-propia-web` — ⚠️ **PÚBLICO**.
- **Online**: **https://convozpropia.es** (GitHub Pages; `CNAME` en el repo). HTTPS + www→apex.
- Estructura: `index.html` (landing) · `demo.html` (escaparate de la app) · `blog/` · `legal/` ·
  `acceso.html` (redirige a la app) · `css/` · `assets/` (og-image) · `404.html` · `sitemap.xml` · `robots.txt`.
- El logo va como **SVG inline** en cada página (no depende de ningún archivo externo).

## Regla de oro de seguridad (repo PÚBLICO)

- **Aquí SOLO va la web pública.** El material de Macu (temario, presentaciones, supuestos) y
  **cualquier dato de alumnado NUNCA** entra en este repo. La demo usa solo datos ficticios.
- **Datos personales autorizados a publicar** (decisión de Miguel, 05-jul-2026): SOLO el nombre
  "Macu" (sin apellidos) y el email de contacto de marca `convozpropiaopos@gmail.com` (creado
  05-jul-2026; sustituyó al personal). **Nada localizable**: ni teléfono/WhatsApp, ni apellidos,
  ni localidad exacta. Contacto de la web: solo email e Instagram. Ningún otro dato sin OK explícito.
- Antes de `git commit`: `git status` + revisar que no se cuela nada sensible. `.gitignore` robusto +
  hook global (`~/.git-hooks/pre-commit`) son barreras, no excusa para no mirar.

## Publicar

```
git add -A && git commit -m "..." && git push    # GitHub Pages actualiza en 1-2 min
```

## Enlace con la app

El botón **"Acceder"** (7 páginas) enlaza a **https://app.convozpropia.es** (login de la plataforma).
`acceso.html` también redirige ahí (por si hay enlaces viejos).
