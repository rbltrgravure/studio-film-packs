# Packs Studio Film · SVG & Images IA

Packs JSON (lecture seule) utilises par le logiciel **Studio Film · SVG & Images IA**.
Depot public : aucun jeton necessaire.

## Packs disponibles

| Fichier | Usage |
|---|---|
| `packs/exemple-pack-studio-film.json` | Pack de demonstration generaliste (2 styles, 3 beats, 11 cadrages, 4 consignes, 2 motifs) |
| `packs/pack-storyboard-viral.json` | **Storyboard viral 9:16** — styles energetiques, cadrages verticaux, beats viraux en 5 temps, regles de surimpression video |
| `packs/pack-documentaire.json` | **Reportage documentaire** — photojournalisme, regard sobre, beats de temoignage, regles de verifiabilite |
| `packs/pack-publicite-produit.json` | **Publicite produit** — packshot et lifestyle, cadrages produit, beats de conversion, regles anti-superlatifs |

## Brancher ce depot

Dans le logiciel : menu **⛁ Bases GitHub**, puis :

| Champ | Valeur |
|---|---|
| Proprietaire | `rbltrgravure` |
| Depot | `studio-film-packs` |
| Fichier | `packs/exemple-pack-studio-film.json` (ou un autre pack de la liste) |
| Branche | `main` |

Puis **Ajouter la source** et **Synchroniser maintenant**.

URL brute : `https://raw.githubusercontent.com/rbltrgravure/studio-film-packs/main/packs/exemple-pack-studio-film.json`

Plusieurs packs peuvent etre branches en meme temps : ils sont fusionnes (styles, cadrages, beats, consignes et motifs s'additionnent).

## Sections d un pack

| Section | Effet |
|---|---|
| `styles[]` | styles visuels ajoutes a la galerie (id, name, desc, prompt, swatch, icon) |
| `shots` | cadrages camera : scales, angles, postures, gazes, micro |
| `beats[]` | beats narratifs : shot, decor, light, expr, desc, narr (champs `{S}`, `{C1}`, `{C2}` acceptes) |
| `rules.scenario` | consigne du prompt de scenario (francais) |
| `rules.case` | consigne du prompt de chaque case (anglais) |
| `rules.character` | consigne des portraits de personnages (anglais) |
| `rules.film` | consigne du plan et des images du film (francais) |
| `svg.patterns[]` | motifs SVG injectes dans les scenes du film (defs = `<pattern>`) |

Toutes les sections sont facultatives.
