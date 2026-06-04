# 🍷 Burgundy Producer Tiers

An interactive, single-file chart that ranks Burgundy wine producers by **quality and prestige** — not by appellation. It maps producers onto **two parallel ladders**, the *négociant* (red) and the *domaine* (purple), and shows why even a great négociant gets **capped** below the cult estates at the top.

> **Live demo:** enable GitHub Pages (see below), then open `index.html`.

---

## The idea

Burgundy is sliced two completely different ways, and people constantly mix them up:

1. **The dirt (AOC classification)** — *what's in the bottle, by vineyard:* Bourgogne → Village → Premier Cru → Grand Cru.
2. **The producer (who made it)** — *the quality and reputation of the house itself.*

This chart is about the **second** axis. And on that axis, producers split into two worlds:

| | Négociant | Domaine |
|---|---|---|
| **What it is** | Buys grapes / juice / wine from growers, then bottles under its own name | Grows its own fruit and estate-bottles it |
| **Label tell** | *"Maison …"* / *"Mis en bouteille par …"* | *"Mis en bouteille au domaine"* |
| **Best example here** | Pierre-Yves Colin-Morey, Maison Leroy, Louis Jadot | DRC, Rousseau, Roumier, d'Angerville |
| **Prestige ceiling** | **Capped** below the apex | Reaches the very top |

### The cap

A house like **Louis Jadot** can be a genuinely *top producer* — legendary winemaking, a full Grand Cru range, and it even owns serious vineyards. But Burgundy's prestige (and price) ceiling rewards tiny, grower-controlled, vine-to-bottle estates. So a négociant — however good — tops out **below** the domaine apex, where **Domaine de la Romanée-Conti (DRC)** sits alone at \$5,000+.

That's the whole point of the chart: the négociant ladder physically can't reach the top. The top quarter is **domaine-only territory**.

```
 NÉGOCIANT (red)              DOMAINE (purple)
 ───────────────             ────────────────
                                   ♛ DRC  ($5k+)               ┐
       (empty —                    Leroy 97                    │
        négociants                 Liger-Belair 96             │ top 25%:
        can't reach                Roumier 95                  │ domaine-only
        the apex)                  Rousseau 94 · Mugnier 94    │ (the "cap")
                                   Coche-Dury 93 · Dujac 93    │
                                   Leflaive 92 · de Vogüé 92   │
                                   Clos de Tart 91             ┘
 - - - - - - - - - - - - - - - - - - - - - - - -  ◄ négociant ceiling (¾ up)
   Maison Leroy 89                 Fourrier 89
   PYCM ★ 88                       d'Angerville 86
   Lucien Le Moine 85              Castagnier 73
   Drouhin 80                      Thévenet 70
   Louis Jadot ★ 78                J-M Guillon 66
   Bouchard 77                     Ravaut 62
   Faiveley 76                     A. & A. Chopin 56
   Louis Latour 72                 Charton 51
   Albert Bichot 60
   Nuiton-Beaunoy 25  (co-op floor)
```

---

## Features

- **Dual quality ladders** — négociant vs domaine, side by side, sharing one quality axis so heights are directly comparable.
- **Non-linear scale** — the elite end is expanded: scores **90–100 fill the top quarter** of the chart, so the cult cluster has room to breathe while the sparse low end is compressed.
- **The cap, made literal** — a dashed "négociant ceiling" line at ¾ height; everything above it is domaine-only, topped by DRC.
- **Click / hover any producer** for a detail card: region, ownership, key Grand Crus, and *why* it sits where it sits.
- **Hybrids flagged** (`H`) — PYCM, Castagnier, Jadot, Faiveley and others both own vineyards *and* buy fruit; the pure categories are rarer than people think.
- **Your named producers highlighted** in gold.
- **Zero dependencies** — one self-contained HTML file. No build step, no libraries, no network calls. Works offline.

---

## Producers included

**Domaine ladder:** Domaine de la Romanée-Conti · Leroy · Comte Liger-Belair · Georges Roumier · Armand Rousseau · J.F. Mugnier · Coche-Dury · Dujac · Leflaive · Comte Georges de Vogüé · Clos de Tart · Fourrier · Marquis d'Angerville · Domaine Castagnier · Domaine de la Bongran (Jean Thévenet) · Jean-Michel Guillon & Fils · Gaston & Pierre Ravaut · A. & A. Chopin · Vincent & Jean-Pierre Charton

**Négociant ladder:** Maison Leroy · Pierre-Yves Colin-Morey · Lucien Le Moine · Joseph Drouhin · Louis Jadot · Bouchard Père et Fils · Faiveley · Louis Latour · Albert Bichot · Nuiton-Beaunoy (co-op)

> Many of the blue-chip domaines (DRC, Leroy, Roumier, Rousseau, Faiveley, Lucien Le Moine, Leflaive) and the additions from Christie's "top Burgundy producers" list (Dujac, de Vogüé, J.F. Mugnier, Comte Liger-Belair, Clos de Tart, Fourrier) live in the top quarter — the domaine-only zone above the négociant cap.

---

## Viewing it

It's a static page, so anyone can interact with it once it's served as a web page:

**GitHub Pages (recommended)**
1. Push these files to the repo (`index.html` + `README.md`).
2. Repo → **Settings → Pages → Build and deployment → Deploy from a branch** → pick `main` / root.
3. Open `https://<your-username>.github.io/burgundy-producer-tiers/`.

> ⚠️ Viewing the file inside the GitHub repo browser (or the "Raw" link) shows the **source code**, not the rendered page — it has to go through Pages (or Netlify/Vercel drag-and-drop) to be interactive. Locally, just double-click `index.html`.

---

## A note on the scores

The 0–100 numbers are an **editorial reputation/prestige scale** for visual ordering — not an official rating. Placements reflect critical standing and secondary-market prestige as of 2026, and reasonable people will quibble. That's half the fun.

## Sources

- [Négociant & Négociant-Éleveur — WineWiki](https://www.winewithseth.com/winewiki/negociant/)
- [What is a Négociant-Éleveur? — Wine Enthusiast](https://www.wineenthusiast.com/culture/wine/burgundy-negociant-wine-guide/)
- [8 Things to Know About Louis Jadot — VinePair](https://vinepair.com/articles/ntk-louis-jadot/)
- Producer profiles: [Marquis d'Angerville](https://www.rarewineco.com/producer/angerville-volnay/) · [Castagnier](https://grandsbourgognes.com/en/wine-estates/bourgogne/domaine-castagnier-439) · [A. & A. Chopin](https://domaine-chopin.fr/) · [Nuiton-Beaunoy](https://nuiton-beaunoy.fr/en/) · [PYCM](https://chambersstwines.com/blogs/articles/pierre-yves-colin-morey-the-magician-of-white-burgundy) · [Jean-Michel Guillon](https://wineambassadeur.com/winegrowers/domaine-jean-michel-guillon/) · [Gaston & Pierre Ravaut](https://www.domaine-ravaut.fr/) · [Domaine de la Bongran / Thévenet](https://www.bongran.com/en/)
