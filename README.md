# Prueba Lectiva

Base SvelteKit con arquitectura `feature-first/domain-first` para integrar la API de Rick and Morty.

## Run

```bash
npm install
npm run dev
```

## Check

```bash
npm run check
npm run build
```

## Deploy

El proyecto queda desplegado con GitHub Actions en GitHub Pages.

- El workflow esta en `.github/workflows/pages.yml`.
- Para Pages se usa `BASE_PATH=/lectiva2`, que coincide con el nombre del repositorio.
- El build genera una salida estatica en `build/`.

## Estructura

- `src/lib/core`: cliente HTTP, configuracion y adaptadores.
- `src/lib/entities`: tipos y mapeos de dominio.
- `src/lib/features`: features por caso de uso.
- `src/routes`: composicion de rutas y carga de datos.
