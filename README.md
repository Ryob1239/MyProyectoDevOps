# MyProyectoDevOps

Repositorio de práctica académica para organizar las carpetas principales de un proyecto de software y conocer los archivos **README**, **LICENCE** y **.gitignore**.

## Objetivo

Establecer una estructura inicial lista para crecer con código, documentación, recursos gráficos, bases de datos y automatizaciones de GitHub Actions.

> **Estado:** repositorio de ejemplo. Todavía no contiene una aplicación terminada; el flujo de GitHub Actions verifica únicamente la estructura y los archivos requeridos.

## Estructura

```text
MyProyectoDevOps/
├── backend/
│   └── .gitkeep
├── frontend/
│   └── .gitkeep
├── database/
│   └── .gitkeep
├── docs/
│   └── INVESTIGACION_Y_EVIDENCIAS.md
├── images/
│   └── .gitkeep
├── .github/
│   └── workflows/
│       └── validar-estructura.yml
├── README.md
├── LICENCE
└── .gitignore
```

> Git no guarda carpetas vacías. Por eso se incluye `.gitkeep` en los directorios que todavía no tienen archivos.

## ¿Para qué sirve cada carpeta?

| Carpeta | Finalidad |
|---|---|
| `backend/` | Código del servidor, API y lógica de negocio. |
| `frontend/` | Interfaz de usuario y recursos de la aplicación web. |
| `database/` | Esquemas, migraciones y scripts de bases de datos (no contraseñas ni bases reales). |
| `docs/` | Investigación, manuales y documentación de la práctica. |
| `images/` | Imágenes, capturas y recursos gráficos. |
| `.github/workflows/` | Flujos automáticos de GitHub Actions. |

## Archivos principales

- **`README.md`:** presenta el proyecto e indica cómo está organizado.
- **`LICENCE`:** contiene una licencia MIT de ejemplo que permite reutilizar el código bajo sus términos. **Antes de publicarlo, reemplaza `[NOMBRE DEL AUTOR O ENTIDAD]` por el titular correcto**. El nombre convencional es `LICENSE`, pero aquí se usa `LICENCE` conforme a la consigna.
- **`.gitignore`:** indica los archivos locales y temporales que Git debe ignorar, por ejemplo `.env`, `node_modules/` y `__pycache__/`.

## Validación automática

El archivo `.github/workflows/validar-estructura.yml` ejecuta una revisión de carpetas y archivos obligatorios con cada `push`, `pull_request` a `main` o ejecución manual. Para observar el resultado, abre la pestaña **Actions** en GitHub.

## Autor

**Felipe Torres Molina** — Práctica de DevOps, 2026.
