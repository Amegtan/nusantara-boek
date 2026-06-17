# Nusantara companion-site - skeleton v0.1

Lokale skeleton van de companion-site `nusantara-boek.nl`, opgezet op 19 mei 2026 in opstartsessie. Wordt later naar GitHub Pages (of Cloudflare Pages / Netlify) gepusht zodra hosting-keuze definitief is.

## Structuur

```
Site/
├── index.html              landingspagina
├── 404.html
├── robots.txt
├── sitemap.xml
├── README.md               (dit bestand)
├── assets/
│   ├── css/site.css        gedeelde stylesheet
│   └── img/                (leeg - illustraties volgen)
├── tijdlijn/
│   ├── index.html          frame-pagina met iframe naar tijdlijn-nl.html
│   ├── tijdlijn-nl.html    kopie van Boek/0260420_WIU_Tijdlijn_NL_14.html
│   └── tijdlijn-en.html    kopie van Boek/0260420_WIU_Tijdlijn_EN_14.html
├── interconnecties/
│   └── index.html          placeholder - D3-graaf volgt week 0/1
├── over/
│   └── index.html          skeleton-tekst; definitieve versie week 1
└── colofon/
    └── index.html          versiebeheer + licenties + brontypering
```

## Wat staat er

- **5 pagina's** (home, tijdlijn, interconnecties, over, colofon) + 404.
- **Eén stylesheet** met basistypografie, kleurschema, navigatie, banners, kaartrooster en mobile-breakpoint.
- **Twee tijdlijn-HTML-bestanden** ingevoerd (NL_14 + EN_14) via `cp` uit `Boek/`.
- **robots.txt + sitemap.xml** voor SEO-basis.
- **In opbouw-banner** op elke pagina-skeleton om verwachtingen te managen.

## Wat staat er nog niet

- **D3-interconnecties-graaf**: bestand moet uit het boek-werkmap worden geidentificeerd en overgezet (placeholder-tekst staat in `interconnecties/index.html`).
- **Bijlage A.M-events-integratie**: tijdlijn-bestand moet uitgebreid van 159 naar 212 events. Apart werkpad.
- **Open Graph-meta-images**: nog geen og-image.
- **Favicon**.
- **Definitieve over-pagina** (200-300 wrd, mission-statement): week 1.
- **About-pagina inhoudelijke teksten**: skeleton-versie staat.
- **Lighthouse-audit + cross-browser-test**: week 1 (do 21 mei).

## Lokaal testen

Open `index.html` direct in een browser, of serve lokaal:

```bash
cd Site
python3 -m http.server 8000
# Bezoek http://localhost:8000/
```

## Volgende stappen (volgens Bucketlist Week 0)

- Wo 20 mei - tijdlijn + interconnecties-graaf in site plaatsen; relatieve verwijzingen herstellen; 404-pagina (gedaan).
- Do 21 mei - basisstijl, navigatie, Open-Graph-meta, favicon, robots.txt (gedaan), sitemap.xml (gedaan).
- Vr 22 mei - DNS-records aanmaken (zodra hosting-keuze + domein-registratie rond).
- Vr 29 mei - GO-LIVE companion-site (Milestone 1).

## Hosting-keuze

Nog open. Aanbeveling: **GitHub Pages** (gratis, git-flow, geen vendor lock-in). Alternatieven: Cloudflare Pages, Netlify. Beslispunt op de Bucketlist (Week 0, zon 17 mei - inhaalslag).

## Domein

`nusantara-boek.nl` te registreren (~ EUR 10/jaar). DNS-records aanmaken op vr 22 mei (CNAME naar GitHub Pages of A-records); propagatie 24-48u.

## Versie

Skeleton v0.1 - 19 mei 2026 (opstartsessie, Claude Opus 4.7).
