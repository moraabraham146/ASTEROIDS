# Publicación rápida en GitHub Pages

Instrucciones rápidas para publicar este proyecto como sitio web en GitHub Pages.

Requisitos:
- Cuenta en GitHub
- git instalado localmente

Pasos desde la carpeta del proyecto (`C:\Users\IK\Documents\ASTEROIDS`):

```powershell
git init
git branch -M main
git add .
git commit -m "Publicar sitio ASTEROIDS"
# Reemplaza la URL por la de tu repositorio en GitHub
git remote add origin https://github.com/<TU_USUARIO>/<TU_REPO>.git
git push -u origin main
```

Detalles:
- El archivo `index.html` está en la raíz; GitHub Pages publicará ese archivo como la página principal.
- Hay un workflow de GitHub Actions en `.github/workflows/deploy-pages.yml` que subirá y desplegará automáticamente el contenido cuando hagas `push` a `main`.
- Si usas `master` como rama principal, renombra la rama a `main` o edita el workflow para ajustar la rama objetivo.

Consejos:
- Para un dominio personalizado, añade un archivo `CNAME` en la raíz con tu dominio y configura las DNS.
- Si no quieres usar el workflow, ve a `Settings > Pages` en GitHub y selecciona la rama `main` y la carpeta `/ (root)`.

Notas sobre Firebase:
- El sitio intenta cargar módulos de Firebase si encuentra variables de configuración; en ausencia de ellas el juego funciona en modo local sin persistencia.
