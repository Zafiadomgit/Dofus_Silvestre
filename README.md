# Dofus Silvestre: checklist de 0 a 100

Página web estática (un solo archivo, `index.html`) para seguir la ruta completa del Dofus Silvestre con hasta 4 personajes. No necesita compilar nada.

## Subirla a GitHub

**Opción fácil (desde el navegador)**
1. Repositorio: https://github.com/Zafiadomgit/Dofus_Silvestre (público). Cualquiera puede leer los archivos, así que aquí no van datos personales: los nombres de tus personajes se escriben dentro de la página y se guardan solo en tu navegador.
2. **Add file → Upload files** y arrastra `index.html`, `vercel.json`, `.gitignore` y `README.md`.
3. **Commit changes**.

**Opción con git**
```bash
git init
git add .
git commit -m "Checklist Dofus Silvestre"
git branch -M main
git remote add origin https://github.com/Zafiadomgit/Dofus_Silvestre.git
git push -u origin main
```

## Publicarla en Vercel
1. En Vercel: **Add New → Project** y elige el repositorio `dofus-silvestre`.
2. **Framework Preset: Other**. Deja vacíos *Build Command* y *Output Directory*.
3. **Deploy**. Cada `git push` a `main` vuelve a publicar la página solo.

## Cómo se guarda el progreso
- El avance se guarda **en el navegador** (localStorage). Si abres la página en otro PC o navegador, empieza en cero.
- Para pasar el avance de un equipo a otro usa los botones **Exportar progreso** (descarga `dofus-silvestre-progreso.json`) e **Importar progreso** (en el otro equipo).
- Si borras los datos del navegador, pierdes el progreso: exporta de vez en cuando como copia de seguridad.

## Actualizar el contenido
Reemplaza `index.html` por la versión nueva y haz commit: Vercel la publica sola.

## Notas
- La página lleva `noindex`, así que los buscadores no deberían listarla. Quita esa línea del `<head>` si quieres lo contrario.
- Las tipografías (Marcellus y Source Sans 3) se cargan desde Google Fonts; sin conexión se usan tipografías del sistema.
- Es una guía no oficial. Las fuentes son Dofus pour les Noobs, Dofuserie, Millenium, Torrente Arcano y otros; el juego puede haber cambiado desde septiembre de 2026.
