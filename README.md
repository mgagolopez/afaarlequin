# AFA Arlequín – web

Web estática de la Asociación de Familias (AFA) de la EIM Arlequín. Es una copia en un solo archivo (`index.html`) de la web original hecha con WordPress: no necesita servidor, base de datos ni compilación.

## Ver la web en local

Abre `index.html` con doble clic en cualquier navegador.

## Publicarla con GitHub Pages

1. Sube `index.html`, `README.md` y `.nojekyll` a la raíz de un repositorio de GitHub.
2. En el repositorio, ve a **Settings → Pages**.
3. En **Build and deployment**, elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`, y guarda.
4. En un par de minutos la web estará en `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

## Cómo editar el contenido

Todo está en `index.html`. Los puntos que se cambian con más frecuencia están marcados con comentarios:

- **Calendario de Google**: en la sección *Organización*, el `src` del `<iframe>`. Debe ser el ID de un calendario **público** (Configuración del calendario → Integrar calendario).
- **Actas, Cuentas, Junta y Otras actividades**: los `href` de esos enlaces apuntan a documentos de Google Drive. Comprueba que estén compartidos como "Cualquier persona con el enlace".
- **Correos de contacto**: la lista de la sección *Contacta / Opina*.
- **Año del pie de página**: la línea `<footer>` al final.

El archivo `.nojekyll` indica a GitHub Pages que sirva los archivos tal cual, sin procesarlos.
