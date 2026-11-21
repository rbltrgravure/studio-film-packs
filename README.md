# Packs Studio Film · SVG & Images IA

Packs JSON (lecture seule) utilises par le logiciel **Studio Film · SVG & Images IA**.

## Brancher ce depot

Dans le logiciel : menu **⛁ Bases GitHub**, puis :

| Champ | Valeur |
|---|---|
| Proprietaire | `rbltrgravure` |
| Depot | `studio-film-packs` |
| Fichier | `packs/exemple-pack-studio-film.json` |
| Branche | `main` |

Puis **Ajouter la source** et **Synchroniser maintenant**.

URL brute : `https://raw.githubusercontent.com/rbltrgravure/studio-film-packs/main/packs/exemple-pack-studio-film.json`

Depot public : aucun jeton necessaire.

## Sections d un pack

| Section | Effet |
|---|---|
| `styles[]` | styles visuels ajoutes a la galerie |
| `shots` | cadrages camera (scales / angles / postures / gazes / micro) |
| `beats[]` | beats narratifs (decor, lumiere, expression, texte) |
| `rules.scenario` | consigne du prompt de scenario |
| `rules.case` | consigne du prompt de chaque case |
| `rules.character` | consigne des portraits de personnages |
| `rules.film` | consigne du plan et des images du film |
| `svg.patterns[]` | motifs SVG injectes dans les scenes du film |

Toutes les sections sont facultatives.
