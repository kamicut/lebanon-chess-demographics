# Lebanon Chess Demographics

Interactive age/gender participation charts for Lebanon's FIDE-rated chess players, modeled on David Smerdon's [age & gender participation analysis](https://www.davidsmerdon.com/?p=2075).

**[View the live page](https://kamicut.github.io/lebanon-chess-demographics/)**

## What's here

A single self-contained `index.html` (no build step, no external requests, no dependencies) with:

- Two histograms — all FIDE-rated players vs. active-only — broken down by age and gender
- Hover a bar for age, approximate birth year, and player counts
- Click a bar to list the players at that age, with FIDE IDs linking to their ratings profile

## Data & methodology

- Source: [FIDE ratings list](https://ratings.fide.com/download.phtml), downloaded 2026-07-05, filtered to `country = LBN`
- Age = 2026 − FIDE birth year (players with no recorded birth year are excluded)
- "Active" follows FIDE's own activity flag (players flagged inactive are excluded)
- This is a one-off exploratory analysis for a single federation, pulled from the broader dataset maintained in [kamicut/fide-players](https://github.com/kamicut/fide-players)

## Local use

Just open `index.html` in a browser — everything is inlined, so it works offline too.
