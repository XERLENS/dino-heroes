# SESSION_START

Quand l’humain dit « session » ou `/session-start` :

1. Lire dans l’ordre : `docs/INBOX.md`, `docs/STATUS.md`, `docs/DESIGN.md`, `docs/DECISIONS.md`, `docs/BACKLOG.md`
2. Répondre en 8 lignes max :
   - Phase
   - Ticket retenu (1 seul, le P0 le plus haut non coché)
   - Fichiers qui seront touchés
   - Risque / hors-scope
   - Critère de done
   - Comment tester
3. Attendre un OK humain si le ticket n’est pas déjà dans `INBOX.md`
4. Faire le ticket
5. Mettre à jour `STATUS.md` et cocher `BACKLOG.md`
6. Ajouter une ligne datée en bas de `STATUS.md` ou dans un `SESSION_LOG.md` si STATUS dépasse un écran
7. Ne jamais réécrire `DESIGN.md` sauf ticket explicite
