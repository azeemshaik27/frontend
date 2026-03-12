# Frontend App (React + Vite)

Minimal React app with Vite. Fetches products from external API.

## Quick Start

```bash
npm install
npm run dev
```

## Build for Production

```bash
npm run build
```

Outputs optimized static files to `/dist`. Preview locally:

```bash
npm run preview
```

## Deployment

### Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. `vercel --prod`

### Netlify
1. Drag `/dist` to [netlify.com/drop](https://app.netlify.com/drop).
2. Or CLI: `npm i -g netlify-cli`, `netlify deploy --prod --dir=dist`.

### Github Pages
1. Install `gh-pages`: `npm i -D gh-pages`
2. Add to scripts: `"deploy-gh": "gh-pages -d dist"`
3. `npm run build && npm run deploy-gh`

### Custom base path
Edit `vite.config.js` `base` (e.g., `/myapp/`). Rebuild.

## API
Uses `VITE_API_URL` from `.env` (fallback `https://backend-3eoi.onrender.com/store`). Copy `.env.example` to `.env`.

See Vite [deployment docs](https://vite.dev/guide/static-deploy.html).
