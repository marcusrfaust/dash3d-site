# Deploy — Dash3D

## Status
- Build: `npm run build` (verde, via `astro build`)
- Produção: https://dash3d-site.pages.dev/
- Deploy: `wrangler pages deploy dist --project-name=dash3d-site --branch main`

## Conferência realizada
- `dist/index.html`: 1 `<h1>` por página (index e 404), todo `<img>` com atributo `alt`.
- `<html lang="pt-BR">`.
- Título sem emoji: "Dash3D — gestão da fábrica 3D da Focol".
- Tema azul: primary `#2563EB`, secondary `#38BDF8` (src/config/theme.json).
- Homepage (`src/pages/index.astro`): apenas Hero, Statistics, KeyFeatures (5 módulos),
  WhyChooseUs (frota), FAQ, CallToAction (e-mail). Sem Pricing/Testimonials/TrustedClients.
- Screenshots reais via CDP local (porta 9333), sem `browser_exec`:
  `evidence/screenshot-390.png` (390×844) e `evidence/screenshot-1440.png` (1440×900).
- Produção verificada byte a byte contra `dist/index.html` (diff idêntico, 77389 bytes).

## Dados reais usados
15 impressoras (13 Bambu Lab + 2 Snapmaker), 194 placas, 2.952 peças, 5 módulos
(ao vivo, produtos, estoque, custos, histórico). Contato: 3d@focol.ai.
