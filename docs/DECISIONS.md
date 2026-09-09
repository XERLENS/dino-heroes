# DECISIONS — Architecture Decision Records

## ADR-001 — Stack

- Date : 2026-09-09
- Décision : Vite + TypeScript strict + Phaser 3
- Pourquoi : un bot livre un proto plus vite avec scenes / camera / input déjà là
- Conséquence : Pixi / Three interdits tant que le rendu n’est pas le goulot
- Statut : accepté

## ADR-002 — Séparation sim / vue

- Décision : `src/engine` 0 Phaser ; `src/view` Phaser only ; état JSON serializable
- Pourquoi : tests, save, undo, IA, replay
- Statut : accepté

## ADR-003 — MVP contenu

- Décision : 2 factions (Meute Émeraude, Nid des Marais). Ressources : Or, Viande, Os, Ambre (stub). Dwellings T1–T4. Carte ~24×24. Combat sans siège.
- Statut : accepté

## ADR-004 — Source de vérité

- Décision : design dans `docs/`, stats dans `data/*.json`, jamais hardcodées dans `src/`
- Statut : accepté

## ADR-005 — IP

- Décision : systèmes HoMM3 inspirés, zéro nom / sprite / faction Ubisoft
- Titre de travail : Dino Heroes
- Statut : accepté

## ADR-006 — Source durable

- Date : 2026-09-09
- Décision : repo GitHub privé `XERLENS/dino-heroes` = copie durable. `/workspace` Grok Bot peut être cloné depuis ce repo.
- Statut : accepté
