# meximalist.com

Operator surface for **Mauricio Cruz** — Mexican AI operator-builder based in Monterrey.

> Companion to `mexi.wtf` (the builder hub). This site handles B2B contact, case studies,
> press kit, and advisory inquiries. Voice: capitalized, professional-warm, Spanish with
> full diacritics. See `mexiweb3/mexi-design-system` for the brand system that drives both surfaces.

## Pages

```
/                        → Home (hero, work, building, about, press preview, contact)
/work/chapas-burgers     → Case study: Chapas Burgers
/work/casablanca         → Case study: Casablanca
/press                   → Press kit (bios, headshots, logos, appearances)
```

## Stack

- HTML estático + tokens inline (no build, no framework)
- Fonts via Google Fonts CDN (Exo 2, Inter, JetBrains Mono)
- Hosted on Vercel
- Deploy: push to `main` → auto-deploy

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy to Vercel

```bash
vercel --prod
```

Then connect domain `meximalist.com` in Vercel project settings and update DNS.

### DNS (GoDaddy)

Replace the current 301 forward to Linktree with:

| Type | Host | Value |
|---|---|---|
| A | `@` | `76.76.21.21` |
| CNAME | `www` | `cname.vercel-dns.com` |

Remove the existing forward to `linktr.ee/mexiweb3`.

## Content TODO

Several `TBD` markers remain — flagged inline in the HTML:

- [ ] Real metrics for Chapas Burgers (msgs/día, hrs ahorradas, ROI real)
- [ ] Casablanca founder quote authorization
- [ ] Métricas operativas para Casablanca
- [ ] Logo assets para download (SVG + PNG)
- [ ] Talks page (cuando exista la primera)
- [ ] Real link al artículo Medium de Jair Sánchez

## Cross-link

- Builder side: [mexi.wtf](https://mexi.wtf)
- Brand system source of truth: [mexiweb3/mexi-design-system](https://github.com/mexiweb3/mexi-design-system)

## Owner

Mauricio Cruz · `m@meximalist.com` · Monterrey, MX
