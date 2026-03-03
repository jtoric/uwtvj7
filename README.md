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

## Navigacijska mapa

Dijagram pokazuje kako su stranice međusobno povezane:

```
                    ┌──────────────┐
                    │   Početna    │
                    │  index.html  │
                    └──────┬───────┘
                           │
          ┌────────────────┼────────────────┐
          │                │                │
   ┌──────▼───────┐ ┌─────▼──────┐ ┌───────▼──────┐
   │   Programi   │ │   O nama   │ │   Kontakt    │
   │programs.html │ │ about.html │ │contact.html  │
   └──────────────┘ └────────────┘ └──────────────┘

Svaka stranica ima globalnu navigaciju (header) i footer
s linkovima na sve ostale stranice → potpuno povezana mreža.
```

## Tehnologije

- **HTML5** — semantički elementi, pristupačnost (a11y)
- **CSS3** — custom properties, Flexbox, Grid, media queries
- **Bez JavaScripta** — čisti HTML/CSS projekt

## Pristupačnost (a11y)

Projekt od početka prati osnovna pravila pristupačnosti:

- **Skip link** — `<a class="skip-link" href="#main">` na svim stranicama omogućuje
  korisnicima tipkovnice preskakanje navigacije
- **Semantički HTML** — `<header>`, `<nav>`, `<main>`, `<footer>`, `<section>`, `<figure>`
- **aria-label** — razlikuje glavnu navigaciju (`"Glavna navigacija"`) od footer navigacije (`"Footer navigacija"`)
- **aria-current="page"** — označava aktivnu stranicu u izborniku za screen readere
- **Alt tekst** — svaka informativna slika ima smislen `alt` opis
- **figure / figcaption** — slike s opisom grupirane semantički

## Status projekta

| Predavanje | Tema | Status |
|------------|------|--------|
| 1 | HTML struktura + sitemap | ✅ Gotovo |
| 2 | Navigacija + pristupačnost | ✅ Gotovo |
| 3 | Forme + tablice + mediji | ⬜ Planirano |
| 4 | CSS osnove: tipografija i razmaci | ⬜ Planirano |
| 5 | Layout: Flexbox i Grid | ⬜ Planirano |
