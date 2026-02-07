# Liga MX

Sitio estático para ver los partidos de **Liga MX**: equipos, hora y canales de TV. Diseño minimalista y cuadrado (sin bordes redondeados).

- **Stack**: Astro, Tailwind CSS, TypeScript
- **Datos**: JSON en `src/data/liga-mx-hoy.json`

## Desarrollo local

```bash
npm install
npm run dev
```

Abre [http://localhost:4321](http://localhost:4321).

## Actualizar partidos

```bash
npm run update-data
```

Esto sobrescribe `src/data/liga-mx-hoy.json`. Si la estructura de la web cambia, puede ser necesario ajustar el script en `scripts/update-liga-mx.mjs`.

## Build y despliegue (GitHub Pages)

El sitio se despliega automáticamente con GitHub Actions al hacer push a `main`.

**Configuración inicial (solo la primera vez):**

1. En el repo, ve a **Settings → Pages**.
2. En **Source**, selecciona **GitHub Actions**.

Tras cada push a `main`, el workflow compila el sitio y lo publica en `https://pitazo.github.io`.
