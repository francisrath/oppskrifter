# Oppskrifter

Statisk side bygget med [Hugo](https://gohugo.io), publisert til GitHub Pages
av `.github/workflows/publiser.yml` ved push til `master`.

## Legge til en oppskrift

Lag ei mappe under riktig kategori og skriv `index.md`:

```
content/kaker/gulrotkake/
├── index.md
└── gulrotkake.jpg      ← valgfritt
```

```markdown
---
title: Gulrotkake
---

## Bunn
- 4 dl hvetemel
- 3 dl sukker

Bland alt og steik på 175 grader i 40 minutt.
```

Det er hele frontmatteren. Kategorien er mappa, og bildet plukkes opp
automatisk — forsida og kategorisidene oppdaterer seg selv.

**Ingredienser skal være punktlister**, framgangsmåte skal være vanlig tekst.
Knappen «Kopier ingredienser» henter alle punktlistene på sida, så det er den
eneste konvensjonen som betyr noe.

Bildet blir skalert til 1400 px WebP ved bygging, men originalen blir liggende i
git for alltid — hold den gjerne under ~2 megapiksel før du committer.

## Lokalt

```sh
brew install hugo
hugo server
```
