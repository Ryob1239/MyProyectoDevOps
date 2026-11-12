# Investigación: README, LICENCE y .gitignore

**Actividad:** Organización de un repositorio GitHub para DevOps  
**Proyecto:** MyProyectoDevOps  
**Estudiante:** [TU NOMBRE]  
**Fecha:** [FECHA DE ENTREGA]

## 1. Introducción

Un repositorio organizado facilita la colaboración, el control de versiones y la automatización. Los archivos `README.md`, `LICENCE` y `.gitignore` tienen funciones diferentes y complementarias: explicar el proyecto, indicar los permisos legales y evitar registrar archivos innecesarios o sensibles.

## 2. ¿Qué es un README.md?

Es un documento informativo que normalmente aparece en la página principal de un repositorio en GitHub. El nombre significa «léeme». Suele estar escrito en Markdown y comunica el propósito del proyecto, su instalación, su uso, requisitos y personas responsables.

**Aplicación en este proyecto:** el `README.md` describe la estructura de `MyProyectoDevOps`, la finalidad de sus carpetas y los pasos para publicarlo en GitHub.

## 3. ¿Qué es un archivo LICENSE o LICENCE?

Es el documento que establece qué permisos y condiciones de uso, modificación y redistribución tienen otras personas respecto al software. Un repositorio público no significa automáticamente que cualquiera pueda reutilizar su código sin restricciones.

**Aplicación en este proyecto:** se incluye un archivo llamado `LICENCE`, tal como solicita la consigna, con el texto de la licencia MIT. Antes de su publicación definitiva, debe sustituirse `[NOMBRE DEL AUTOR O ENTIDAD]` por el verdadero titular de los derechos. La denominación `LICENSE` es la convención más utilizada en GitHub.

**Razón para elegir MIT como ejemplo:** es breve y permisiva, y deja claro que se debe conservar el aviso de derechos de autor y de licencia.

## 4. ¿Qué es un archivo .gitignore?

Es un archivo de configuración con patrones que indican a Git qué archivos o carpetas no debe empezar a rastrear. Es útil para archivos temporales, entornos virtuales, dependencias descargadas, registros y secretos que se guardan localmente.

**Aplicación en este proyecto:** se ignoran `.env`, `node_modules/`, `__pycache__/`, `.venv/`, archivos `.log` y bases de datos locales. Importante: agregar algo a `.gitignore` **no elimina del historial** archivos que ya se habían subido. Si se publicó accidentalmente un secreto, se debe revocar o cambiar también.

## 5. Organización del repositorio

| Elemento | Función |
|---|---|
| `backend/` | Código del servidor o lógica de negocio. |
| `frontend/` | Pantallas y recursos de la interfaz. |
| `database/` | Scripts y esquemas de datos. |
| `docs/` | Documentación y evidencia de la práctica. |
| `images/` | Imágenes del proyecto y capturas. |
| `.github/workflows/` | Automatizaciones mediante GitHub Actions. |
| `README.md` | Presentación y guía de uso. |
| `LICENCE` | Condiciones de licencia. |
| `.gitignore` | Archivos que Git debe ignorar. |

Los archivos `.gitkeep` son marcadores que permiten versionar carpetas que, de otro modo, estarían vacías.

## 6. Automatización con GitHub Actions

Se agregó `.github/workflows/validar-estructura.yml`. Este flujo inicia con cada subida a `main`, una solicitud de extracción (*pull request*) hacia `main` o una ejecución manual. El trabajo usa un ejecutor de Ubuntu, descarga el código mediante `actions/checkout` y comprueba que todas las carpetas y archivos solicitados existen. Si falta alguno, termina con error; de lo contrario, finaliza correctamente.

No se ejecutan pruebas funcionales porque todavía no se proporcionó una aplicación; esta automatización es una comprobación de estructura.

## 7. Evidencias que debes capturar en tu cuenta de GitHub

**Evidencia 1 — Repositorio creado.** Captura la vista principal donde se vean el nombre `MyProyectoDevOps`, la rama `main` y los directorios principales.

**[INSERTAR AQUÍ CAPTURA 1]**

**Evidencia 2 — README visible.** Captura el texto de `README.md` mostrado debajo del listado de archivos en GitHub.

**[INSERTAR AQUÍ CAPTURA 2]**

**Evidencia 3 — LICENCE.** Abre `LICENCE` y captura su contenido, incluyendo el encabezado `MIT License` y el nombre del titular ya corregido.

**[INSERTAR AQUÍ CAPTURA 3]**

**Evidencia 4 — .gitignore.** Abre `.gitignore` y muestra varias reglas de exclusión.

**[INSERTAR AQUÍ CAPTURA 4]**

**Evidencia 5 — Workflow.** Entra a `.github/workflows/validar-estructura.yml` y captura su contenido o su ruta.

**[INSERTAR AQUÍ CAPTURA 5]**

**Evidencia 6 — Ejecución de Actions.** En la pestaña `Actions`, abre «Validar estructura del repositorio» y captura el trabajo de verificación exitoso (marca verde) y sus pasos.

**[INSERTAR AQUÍ CAPTURA 6]**

**Enlace al repositorio:** [PEGAR ENLACE REAL DE GITHUB]

## 8. Conclusión

El uso conjunto de `README.md`, `LICENCE` y `.gitignore` mejora la comunicación técnica, define cómo puede usarse el software y reduce la inclusión accidental de archivos locales en el control de versiones. La estructura separada para backend, frontend, base de datos, documentación e imágenes permite que el proyecto crezca de manera ordenada. Además, un flujo sencillo de GitHub Actions permite comprobar automáticamente que la organización básica se mantenga.

## 9. Referencias

- GitHub Docs. (s. f.). *About the repository README file*. https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes
- GitHub Docs. (s. f.). *Licensing a repository*. https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository
- GitHub Docs. (s. f.). *Ignorar archivos*. https://docs.github.com/es/get-started/git-basics/ignoring-files
- GitHub Docs. (s. f.). *Quickstart for GitHub Actions*. https://docs.github.com/en/actions/get-started/quickstart
