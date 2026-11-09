# User Stories — Centre de don de sang

## Règles de rédaction
- Une story traduit un besoin **explicitement présent dans la demande client**, avec sa phrase source.
- Aucune règle du client n'est inventée : ce qui n'est pas confirmé devient un point ouvert dans [`../questions-client.md`](../questions-client.md).
- Les critères marqués `[à valider]` ou `[point ouvert]` dépendent des réponses du client et ne doivent pas être codés tels quels.
- La finalité (« afin de ») est écrite seulement si la demande la donne ; sinon `[finalité à valider avec le client]`.
- Les priorités ne viennent pas du client : elles restent « à valider ».

## Index

| ID | Rôle | Story | Exigence TP1 | Priorité | Statut |
|---|---|---|---|---|---|
| [US-01](US-01-prendre-rendez-vous.md) | donneur | Prendre rendez-vous pour un don | REQ-F-01 | À valider | À préciser |
| [US-02](US-02-verifier-eligibilite.md) | infirmier | Vérifier si un donneur peut donner | REQ-F-02 | À valider | À préciser |
| [US-03](US-03-gerer-dossiers-donneurs.md) | médecin | Gérer les dossiers des donneurs | REQ-F-03 | À valider | À préciser |
| [US-04](US-04-suivre-collectes.md) | responsable des collectes | Suivre les collectes | REQ-F-04 | À valider | À préciser |
| [US-05](US-05-frequence-des-dons.md) | médecin `[rôle à valider]` | Empêcher les dons trop fréquents | REQ-F-05 | À valider | À préciser |
| [US-06](US-06-groupe-sanguin-manquant.md) | donneur d'un groupe sanguin qui manque | Venir très vite quand mon groupe sanguin manque | Aucune exigence validée (voir TP1, Q5 et Q8) | À valider | À préciser |
| [US-07](US-07-proteger-donnees.md) | donneur | Protéger mes données | REQ-NF-01 | À valider | À préciser |

## Éléments volontairement non transformés en stories
- **Débordement de la salle de prélèvement** : problème cité, aucune fonction demandée (Q-29, Q-30, Q-31).
- **Gestion des réserves de sang** : non demandée (Q-42).
- **Rappel automatique, questionnaire de santé en ligne, application mobile native, double authentification et chiffrement** : rejetés dans l'analyse IA du TP1.
- **Alerte automatique SMS/e-mail, plafond de rendez-vous par créneau, gestion complète des stocks** : « À valider » dans l'analyse IA du TP1 ; pas de story avant réponse du client.
