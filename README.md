# EXATEC Suiza

Sitio de la comunidad EXATEC Suiza: quiénes somos, mapa de capítulos regionales, mesa directiva, eventos y el Encuentro EXATEC Suiza 2027.

Es un sitio estático de una sola página (`index.html`), sin build ni dependencias — se puede abrir directo en el navegador o publicar en GitHub Pages.

## Estructura

```
exatec-suiza-site/
├── index.html
├── README.md
└── img/
    ├── logo.png
    ├── comunidad-grupo.jpg
    ├── oeschinensee.jpg
    └── team/
        ├── ana-de-la-fuente.jpg ... (mesa directiva 2026–2028)
        └── mesa-fundadora/
            └── gerardo-garcia.jpg ... (mesa directiva 2022–2025)
```

## Subirlo a un repositorio nuevo en GitHub

### 1. Crea el repositorio en GitHub

En [github.com/new](https://github.com/new): ponle un nombre (por ejemplo `exatec-suiza`), déjalo público o privado según prefieras, y **no** marques "Add a README" ni ".gitignore" (ya los traemos). Clic en **Create repository**.

### 2. Desde esta carpeta, en tu terminal

```bash
cd exatec-suiza-site

git init
git add .
git commit -m "Primera versión del sitio EXATEC Suiza"
git branch -M main

# Reemplaza TU-USUARIO y el nombre del repo por los tuyos:
git remote add origin https://github.com/TU-USUARIO/exatec-suiza.git
git push -u origin main
```

Si usas SSH en vez de HTTPS:

```bash
git remote add origin git@github.com:TU-USUARIO/exatec-suiza.git
```

### 3. Publícalo con GitHub Pages (opcional, para tener un link público)

1. En GitHub, entra a **Settings → Pages** del repositorio.
2. En "Build and deployment" → **Source**, elige **Deploy from a branch**.
3. En **Branch**, elige `main` y la carpeta `/ (root)`. Guarda.
4. En un par de minutos el sitio queda disponible en:
   `https://TU-USUARIO.github.io/exatec-suiza/`

## Editar contenido

Todo el texto, los datos de la mesa directiva, los eventos y el mapa están directamente en `index.html` (HTML + CSS + JavaScript en un solo archivo, sin frameworks). Para cambiar una foto, reemplaza el archivo correspondiente dentro de `img/` manteniendo el mismo nombre, o cambia la ruta en el `<img src="...">` correspondiente.

La foto de Oeschinensee en la pestaña "Encuentro 2027" es una imagen de referencia — está marcada como pendiente de reemplazar por una foto real de la sede del encuentro cuando se confirme.
