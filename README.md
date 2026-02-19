# Training Programs Library

Statički HTML/CSS web izrađen u sklopu kolegija
**Uvod u web tehnologije** na Sveučilištu u Zadru.

Stranica prikazuje fiktivnu platformu za programe obuke — četiri stranice
koje demonstriraju semantički HTML, pristupačnost (a11y), moderan CSS layout
(Flexbox + Grid), responzivni dizajn i CSS-only hamburger izbornik.

## Mapa stranica (sitemap)

```
Početna (index.html)
├── Hero sekcija
├── Istaknuti programi
└── Pregled pogodnosti

Programi (pages/programs.html)
├── Katalog programa (grid kartice)
├── Detalji programa (kratko)
└── Tablica rasporeda

O nama (pages/about.html)
├── O platformi
├── Tim
└── Vizija / misija

Kontakt (pages/contact.html)
├── Kontakt forma (s validacijom)
└── Osnovne kontakt informacije
```

## Struktura projekta

```
/
├── index.html              ← Početna stranica
├── pages/
│   ├── programs.html       ← Katalog programa
│   ├── about.html          ← O nama
│   └── contact.html        ← Kontakt forma
├── styles/
│   ├── tokens.css          ← Design tokeni (boje, razmaci…)
│   ├── base.css            ← Reset, osnovni stilovi, linkovi
│   ├── layout.css          ← Header, footer, sekcije
│   ├── components.css      ← Gumbi, kartice, forme
│   └── pages.css           ← Stilovi specifični za pojedine stranice
├── assets/
│   ├── img/                ← Slike
│   └── icons/              ← Ikone (SVG i sl.)
└── README.md
```

## Tehnologije

- **HTML5** — semantički elementi, pristupačnost (a11y)
- **CSS3** — custom properties, Flexbox, Grid, media queries
- **Bez JavaScripta** — čisti HTML/CSS projekt
