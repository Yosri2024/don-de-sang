# US-05 — Empêcher les dons trop fréquents

**En tant que médecin `[rôle à valider]`**, **je veux** ne pas pouvoir accepter un donneur plus souvent que la fréquence autorisée, **afin de** protéger la santé des donneurs.

| Champ | Valeur |
|---|---|
| ID | US-05 |
| Source | « Il faut protéger la santé des donneurs, qui ne doivent pas donner trop souvent dans l'année » |
| Exigence liée | REQ-F-05 |
| Priorité | À valider avec le client |
| Statut | À préciser |

## Critères d'acceptation provisoires

- [ ] Le système contrôle la fréquence des dons d'un donneur. `[à valider : au rendez-vous ou à l'arrivée]`
- [ ] L'intervalle minimal appliqué est celui retenu par le client (3 mois ou 8 semaines). `[point ouvert]`
- [ ] Le nombre maximal de dons par an est celui validé par le client. `[point ouvert]`
- [ ] Le comportement en cas de dépassement (refus ou exception) est défini avec le client. `[point ouvert]`

## Points ouverts

- Q-07 : 3 mois ou 8 semaines ?
- Q-08 : qui tranche ?
- Q-10 : maximum annuel ?
- Q-12 : année civile ou glissante ?
- Q-13 : refus ou exception ?
- Q-14 : date de réservation ou de rendez-vous ?

## Traçabilité

| Besoin métier | Objectif | Exigence | Source |
|---|---|---|---|
| Empêcher les dons trop fréquents | OBJ-01 | REQ-F-05 | « Il faut protéger la santé des donneurs, qui ne doivent pas donner trop souvent dans l'année » |
