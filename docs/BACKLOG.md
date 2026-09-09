# BACKLOG

Règle ticket : un ID, un fichier principal, un critère de done testable en 3 clics.

## P0 — proto cliquable

- [x] P0-00 Cerveau fichiers (ce repo)
- [ ] P0-01 Scaffold Vite+TS+Phaser, scripts `dev`/`build`, tsconfig strict
- [ ] P0-02 `src/engine/hex.ts` axial + neighbors + distance + tests
- [ ] P0-03 `GameState` serializable + reducer `END_TURN`
- [ ] P0-04 AdventureScene : grille 24×24, camera, clic sélectionne tuile
- [ ] P0-05 1 héros, points de mouvement, pathfinding A* terrain plat
- [ ] P0-06 Ressources joueur + 2 mines capturables
- [ ] P0-07 1 nid : hall + dwelling T1 + dwelling T2, 1 build/jour
- [ ] P0-08 CombatScene hex 15×11, 2 stacks vs 2, initiative, attaque/riposte
- [ ] P0-09 Save/load localStorage (GameState JSON)
- [ ] P0-10 Brancher placeholders unités des 2 factions T1–T3 depuis `data/`

## P1 — après proto

- [ ] Fog of war
- [ ] IA « attaque le plus proche »
- [ ] T4 + 2 bâtiments nid
- [ ] 2 sorts Instinct / 2 sorts Cataclysme
