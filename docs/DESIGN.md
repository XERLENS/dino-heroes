# Dino Heroes — DESIGN.md

Statut : v0 figée pour le proto. Toute modification = ticket + ligne dans `DECISIONS.md`.

## Vision

TBS navigateur inspiré des 3 piliers HoMM3 (aventure, combat hex, villes),
thème dinosaures original. Titre de travail : **Dino Heroes**.
Pas de noms / sprites / cartes Ubisoft.

## Piliers

1. Carte d'aventure tour par tour (hex, fog, mines, objets)
2. Combat hex tactique séparé (initiative, stacks)
3. Nids : 1 bâtiment / jour, dwellings, recrutement
4. Héros + armée (max 7 stacks plus tard ; MVP = 2)

## Scope MVP (figé)

- Carte 24×24, 1 niveau, pas de souterrain
- 1 héros joueur + 1 héros IA bête
- 2 factions : Meute Émeraude (rush) + Nid des Marais (tank)
- Unités T1–T3 seulement (T4 stub JSON autorisé, pas jouable)
- Ressources : Or, Viande, Os (Ambre = stub, pas utilisée)
- Magie : 0 sort au proto (école Instinct réservée)
- Combat : 15×11 hex, pas de siège, pas de sorts
- Save/load JSON localStorage
- Art : placeholders géométriques colorés + nom

## Factions MVP

### Meute Émeraude

- Identité : raptors, vitesse, bonus pack si alliés adjacents
- Héros signature : Veyra l’Alpha (primaire Attaque)
- Terrain natal : jungle
- Couleur placeholder : `#2E8B57`

### Nid des Marais

- Identité : ankylos / spinos, armure, contrôle de zone
- Héros signature : Mora la Mère-Nid (primaire Défense)
- Terrain natal : marais
- Couleur placeholder : `#4A5D23`

## Économie proto

- Or : revenu nid + mines d’or
- Viande : mines / carcasses (recrutement)
- Os : carrières (bâtiments)
- 1 mine = +1 ressource / jour si contrôlée
- Hall de nid : +500 or / jour

## Victoire proto

Éliminer le héros ennemi **ou** capturer son nid.

## Hors scope

Interdit tant que le proto n’est pas jouable 10 minutes :
3D, multi, 8 factions, T5–T7, sièges, campagne, génération XL, audio final.
