# AGENTS.md — Dino Heroes

Source de vérité des **règles**. Le contenu du jeu est dans `docs/` et `data/`.

## Studio

- **Rex** — producer. Assigne, refuse le scope creep, ne code pas (sauf si Forge est absent).
- **Sauria** — design. Écrit `docs/` et propose du JSON. Jamais de code moteur.
- **Forge** — engine. Implémente un ticket à la fois dans `src/`. Ne change pas les stats.
- **Flint** — content / QA. Remplit `data/`, placeholders, playtest. N'invente pas de mécanique.

## Stack imposée

Vite + TypeScript strict + Phaser 3.

- `src/engine/` — règles pures, testables, **0 Phaser**
- `src/view/` — scènes Phaser seulement
- `src/ui/` — overlays HTML/CSS
- `data/*.json` — unités, factions, bâtiments, sorts, cartes

État de jeu serializable (save, undo, tests, IA).

## Loop de session

Lire dans l'ordre : `docs/INBOX.md` → `docs/STATUS.md` → `docs/DESIGN.md` → `docs/DECISIONS.md` → `docs/BACKLOG.md`.

1. Un ticket par session.
2. Faire tourner le proto / les tests.
3. Mettre à jour `STATUS.md`.
4. Cocher le ticket dans `BACKLOG.md` et `INBOX.md` (ne jamais effacer l'historique).
5. `DESIGN.md` se réécrit rarement. Tout changement de proto passe par `DECISIONS.md`.

## Interdits

- Hardcoder des stats dans `src/`
- Nouvelle faction ou 5e ressource sans ADR
- Refactor hors ticket
- Assets / noms HoMM3 (IP Ubisoft)
- Publier, merger destructif, ou lock de balance sans OK humain
- Bloquer sur l'art : placeholders géométriques = OK

## Langues

FR pour le design et la comm. EN pour le code (idents, comments courts).

## Done

Chaque ticket dit comment tester en 3 clics.
