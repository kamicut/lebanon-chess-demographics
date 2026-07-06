# Lebanon Chess Demographics

Interactive age/gender participation charts for Lebanon's FIDE-rated chess players, modeled on David Smerdon's [age & gender participation analysis](https://www.davidsmerdon.com/?p=2075).

**[View the live page](https://kamicut.cc/lebanon-chess-demographics/)**

## What's here

A single self-contained `index.html` (no build step, no external requests, no dependencies) with:

- One histogram of Lebanon's FIDE players by age and gender, defaulting to players who are both currently active and have received at least one published rating
- A toggle to "Include all registered and inactive players," bringing back everyone who's ever been issued a FIDE ID under Lebanon, including the roughly two-thirds who never received a rating
- Hover a bar for age, approximate birth year, and player counts
- Click a bar to list the players at that age, with FIDE IDs linking to their ratings profile

## Data & methodology

- Source: [FIDE ratings list](https://ratings.fide.com/download.phtml), downloaded 2026-07-05, filtered to `country = LBN`
- Age = 2026 − FIDE birth year (players with no recorded birth year are excluded)
- "Active" follows FIDE's own activity flag; "rated" means the player has a nonzero standard, rapid, or blitz rating
- The default view (active + rated) and the "include all" toggle were collapsed from an earlier two-chart design once it became clear the all-vs-active split barely mattered. Inactive players are only about 7% of registrations, dwarfed by the roughly 64% who were never rated at all
- This is a one-off exploratory analysis for a single federation, pulled from the broader dataset maintained in [kamicut/fide-players](https://github.com/kamicut/fide-players)

## Local use

Just open `index.html` in a browser. Everything is inlined, so it works offline too.
