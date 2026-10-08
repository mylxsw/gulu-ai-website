# Gulu AI website

The company homepage for [gulu.ai](https://gulu.ai), built with React, TypeScript and Vite.

## Develop

```bash
npm install
npm run dev       # http://localhost:5173
npm run build     # type-check and build to dist/
npm run preview   # serve the production build
npm run lint
```

`dist/` is a static site. Deploy it to any static host (Cloudflare Pages, Vercel, Netlify, Nginx).

## Editing content

- **Products:** `src/data/products.ts`. The first product with `featured: true` is the large card. To use a real logo, put the image in `public/logos/` and set `logo: '/logos/<file>.png'`. Without a logo, the card shows the two-letter `monogram`.
- **Navigation, model list, contact email:** `src/data/site.ts`. The contact email is a placeholder; replace it before launch.
- **Colors and fonts:** the tokens at the top of `src/styles/global.css`.

## Structure

```
src/
  App.tsx              page sections in order
  data/                products and site content
  components/          one component (and its CSS) per section
  styles/global.css    design tokens and shared styles
```
