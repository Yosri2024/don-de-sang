**TP1 — Cadrage du projet : Centre de don de sang (éligibilité des donneurs)**  
   
 Équipe : Yosri Dkhil, Amine Aslouj , Oumayma Baghoudi , Mohamed Nejib Chabbouh  
   
 **1. Vision**  
   
 **Q1 — Problème métier**  
   
 Le centre ne dispose pas d'un moyen fiable de faire respecter la fréquence des dons, d'absorber l'affluence de la salle de prélèvement et de faire venir rapidement les donneurs d'un groupe sanguin qui manque, alors que ses réserves manquent souvent.  
   
 **Phrase qui décrit une solution :** « Le centre veut une application pour ses donneurs de sang. »  
   
 **Q2 — Parties prenantes**  
  
|  |  |  |  
| - | - | - |  
|   |    |    |  
| **Partie prenante** |  **Statut** |  **Attente** |  
| Donneur |  Explicite |  Prendre rendez-vous pour un don |  
| Infirmier |  Explicite |  Vérifier si un donneur peut donner |  
| Médecin |  Explicite |  Gérer les dossiers des donneurs ; au moins 3 mois entre deux dons |  
| Responsable des collectes |  Explicite |  Suivre les collectes ; accepter un donneur toutes les 8 semaines |  
| Centre de transfusion (commanditaire) |  Explicite |  Une application ; protéger les donneurs ; données protégées |  
| Service informatique ou prestataire |  Potentielle |  Exploitation, maintenance |  
  
   
   
   
 **Q3 — Objectifs**  
- **OBJ-01** — Réduire le nombre de dons acceptés en dehors de la fréquence autorisée de \[valeur actuelle à mesurer\] à \[valeur cible à valider\] d'ici \[délai à valider\].  
- **OBJ-02** — Réduire le nombre de matinées où la salle de prélèvement déborde de \[valeur actuelle à mesurer\] à \[valeur cible à valider\] d'ici \[délai à valider\].  
   
 Les valeurs `[à valider]` font l'objet de questions dédiées dans `questions-client.md` (section « Valeurs des objectifs »).  
 **Q4 — Objectif le plus difficile à mesurer**  
 **Protéger la santé des donneurs.** Difficile à mesurer parce que la « santé » est une notion large et subjective : le client n'a donné ni indicateur, ni valeur, ni règle de fréquence précise (3 mois ou 8 semaines, maximum annuel absent). Indicateurs possibles à proposer au client : proportion de dons conformes à la règle de fréquence retenue ; nombre de dons acceptés malgré un non-respect de cette règle ; nombre de refus d'éligibilité posés par l'infirmier. Aucune valeur cible sans confirmation du client.  
 **2. Périmètre**  
 **Q5 — Tableau connu / inconnu**  
  
|  |  |  |  
| - | - | - |  
|   |    |    |  
| **Élément** |  **Catégorie** |  **Source (phrase de la demande) ou « à valider »** |  
| Prendre rendez-vous pour un don |  Dans le périmètre |  « Les donneurs doivent pouvoir prendre rendez-vous pour un don » |  
| Vérifier si un donneur peut donner |  Dans le périmètre, à préciser |  « l'infirmier doit vérifier si un donneur peut donner » ; critères non fournis |  
| Gérer les dossiers des donneurs |  Dans le périmètre, à préciser |  « Le médecin veut gérer les dossiers des donneurs » ; « gérer » ambigu |  
| Suivre les collectes |  Dans le périmètre, à préciser |  « Le responsable des collectes veut suivre les collectes » |  
| Donneurs d'un groupe manquant : venir très vite |  Dans le périmètre, à préciser (pas encore d'exigence : voir Q7 et Q8) |  « ses donneurs doivent pouvoir venir très vite » ; moyen et délai non précisés |  
| Ne pas donner trop souvent dans l'année |  Règle / exigence initiale |  « qui ne doivent pas donner trop souvent dans l'année » ; sans valeur |  
| Données protégées |  Contrainte / BNF à préciser |  « Les données doivent être protégées » ; non mesurable |  
| « Très vite » |  BNF à préciser |  « venir très vite » ; aucun délai |  
| Intervalle entre deux dons : 3 mois ou 8 semaines |  Point ouvert |  « au moins 3 mois » (médecins) contre « toutes les 8 semaines » (responsable) |  
| Salle de prélèvement qui déborde |  Point ouvert |  « certains matins, la salle de prélèvement déborde » ; aucune fonction demandée |  
| Type d'application et appareils d'accès |  Point ouvert |  « une application » ; aucun appareil imposé |  
| Identification des utilisateurs et droits par rôle |  Point ouvert |  à valider |  
| Annulation ou modification d'un rendez-vous |  Point ouvert |  à valider |  
| Contrôle de fréquence bloquant ou avec exceptions |  Point ouvert |  à valider |  
| Gestion des réserves de sang |  Point ouvert |  « nos réserves manquent souvent » ; gestion non demandée |  
| Le groupe sanguin de chaque donneur est connu et enregistré |  Hypothèse |  à valider |  
| **Point ouvert lié :** où est enregistré le groupe sanguin, et le dossier le contient-il ? |  Point ouvert |  à valider |  
| L'historique des dons passés est disponible et exploitable |  Hypothèse |  un cahier est cité, pas son contenu ; à valider |  
| **Point ouvert lié :** où sont les dons passés, et faut-il les reprendre ? |  Point ouvert |  à valider |  
| Il n'existe qu'un seul type de don |  Hypothèse |  « un don » ; à valider |  
| **Point ouvert lié :** existe-t-il plusieurs types de dons avec des règles différentes ? |  Point ouvert |  à valider |  
| Le centre signale lui-même qu'un groupe manque |  Hypothèse |  origine de l'information non indiquée ; à valider |  
| **Point ouvert lié :** comment le centre constate-t-il qu'un groupe manque ? |  Point ouvert |  à valider |  
  
   
   
   
 **Q6 — Élément hors périmètre**  
   
 Gestion des réserves de sang : classée en **point ouvert**, non exclue. La demande ne demande pas de les gérer mais ne l'exclut pas non plus ; l'exclure serait une décision du client.  
   
 **3. Exigences**  
   
 **Q7 — Tableau des exigences**  
  
|  |  |  |  |  
| - | - | - | - |  
|   |    |    |    |  
| **ID** |  **Exigence** |  **Type** |  **Source** |  
| REQ-F-01 |  Le système doit permettre à un donneur de prendre rendez-vous pour un don. |  F |  « Les donneurs doivent pouvoir prendre rendez-vous pour un don » |  
| REQ-F-02 |  Le système doit permettre à un infirmier de vérifier si un donneur peut donner. |  F |  « l'infirmier doit vérifier si un donneur peut donner » |  
| REQ-F-03 |  Le système doit permettre à un médecin de gérer les dossiers des donneurs. |  F |  « Le médecin veut gérer les dossiers des donneurs » |  
| REQ-F-04 |  Le système doit permettre au responsable des collectes de suivre les collectes. |  F |  « Le responsable des collectes veut suivre les collectes » |  
| REQ-F-05 |  Le système doit empêcher qu'un donneur donne plus souvent que la fréquence autorisée. |  F |  « ne doivent pas donner trop souvent dans l'année » |  
| REQ-NF-01 |  Le système doit protéger les données. |  NF |  « Les données doivent être protégées. » |  
  
   
   
   
 Note : « fréquence autorisée » (REQ-F-05) et « gérer » (REQ-F-03) sont à préciser avec le client. Le besoin « groupe sanguin manquant » est dans le périmètre mais n'a pas d'exigence tant que « très vite » et le moyen de joindre les donneurs ne sont pas définis (voir Q8).  
   
 **Q8 — Critique d'exigences**  
   
 **Exigences du TP :**  
- **REQ-F-06** « Le système doit permettre à l'administration de gérer les salles. » Problème : « gérer » est ambigu (ajouter, modifier, supprimer, rendre indisponible ?). Question au client : quelles opérations la gestion comprend-elle ? (Transposé ici : REQ-F-03.)  
- **REQ-NF-02** « …accessible depuis un ordinateur et un smartphone. » Problème : la demande dit « ordinateur **ou** téléphone », et « smartphone » est un mot ajouté. Version corrigée : « …depuis un ordinateur ou un téléphone », ou question au client.  
 **Exemples sur notre sujet :**  
- « Le système doit refuser tout rendez-vous d'un donneur dont le dernier don date de moins de 3 mois. » Problème : retient la position des médecins et ignore celle du responsable des collectes. Question : quel intervalle retenez-vous, 3 mois ou 8 semaines, et qui tranche ?  
- « Le système doit permettre aux donneurs d'un groupe manquant de venir très vite. » Problème : « très vite » non vérifiable. Questions : quel délai, comment le manque est-il constaté, comment les donneurs sont-ils joints ?  
 **Q9 — « Les données doivent être protégées »**  
   
 Non vérifiable en l'état. Questions au client : quelles données, contre quelles menaces, qui accède à quoi, quelles règles s'appliquent et qui les confirme, quelle durée de conservation, comment vérifier que la protection est suffisante.  
 **4. Analyse IA**  
   
 Prompt utilisé : « Analyse cette demande client pour un système de don de sang. Identifie les ambiguïtés, les informations manquantes et les questions qui devraient être posées au client. N'invente pas de nouvelles exigences. » La sortie ci-dessous a été produite par un assistant IA (Claude) à partir de la demande du sujet 17 ; la classification est la décision humaine.  
 **Q10 — Tableau de classement**  
  
|  |  |  |  
| - | - | - |  
|   |    |    |  
| **Proposition IA** |  **Décision** |  **Justification** |  
| 1. Trancher 3 mois / 8 semaines |  Acceptée |  Contradiction explicite dans la demande |  
| 2. Préciser le maximum annuel de dons |  Acceptée |  « dans l'année » sans valeur |  
| 3. « Dans l'année » : année civile ou 12 mois glissants ? |  Acceptée |  Ambiguïté présente dans le texte |  
| 4. Préciser les critères de l'infirmier |  Acceptée |  « peut donner » non défini |  
| 5. Préciser « gérer les dossiers » |  Acceptée |  Verbe ambigu dans le texte |  
| 6. Annulation ou modification d'un rendez-vous |  À valider |  Plausible, absente de la demande → point ouvert |  
| 7. Plafonner les rendez-vous par créneau |  À valider |  Problème cité (débordement), solution non demandée → question sur la régulation |  
| 8. Alerte automatique SMS/e-mail au groupe manquant |  À valider |  Besoin explicite, moyen non précisé |  
| 9. Gestion complète des stocks de sang |  À valider |  Non demandée → point ouvert |  
| 10. Questionnaire de santé en ligne avant rendez-vous |  Rejetée |  Fonction et contenu médical inventés |  
| 11. Rappel automatique 48 h avant |  Rejetée |  Fonction et délai inventés |  
| 12. Application mobile native iOS et Android |  Rejetée |  Choix technique non demandé |  
| 13. Double authentification et chiffrement |  Rejetée |  Choix techniques prématurés |  
  
   
   
   
 **Q11 — Proposition plausible mais inventée**  
   
 **Proposition 10, le questionnaire de santé en ligne.** Convaincante : elle répond à la protection des donneurs, soulage l'infirmier et semble professionnelle. Dangereuse si acceptée sans vérification : la demande ne dit ni quelles informations recueillir ni qui décide. Elle élargit le périmètre (nouveau parcours, nouvelles données de santé), exige une validation médicale, déplace la décision de l'infirmier vers le système et rend les tests impossibles sans règles validées.  
   
 **Q12 — Ambiguïté relevée par l'IA que nous n'avions pas identifiée**  
   
 « Dans l'année » : année civile ou 12 derniers mois ? Nous avions relevé l'absence de valeur du maximum annuel et la contradiction 3 mois / 8 semaines, mais pas la façon de compter l'année. Une règle sans période claire donne des résultats différents pour un même donneur et n'est pas testable. *(À confirmer par l'équipe : n'écrivez cette réponse que si elle correspond à ce que vous aviez réellement identifié.)*  
   
 **Traçabilité**  
  
|  |  |  |  |  
| - | - | - | - |  
|   |    |    |    |  
| **Besoin métier** |  **Objectif** |  **Exigence initiale** |  **Source dans la demande** |  
| Protéger la santé des donneurs |  OBJ-01 |  REQ-F-05 |  « ne doivent pas donner trop souvent dans l'année » |  
| S'assurer qu'un donneur peut donner |  OBJ-01 (lien à valider) |  REQ-F-02 |  « l'infirmier doit vérifier si un donneur peut donner » |  
| Prise de rendez-vous des donneurs |  Aucun objectif défini (à valider) |  REQ-F-01 |  « Les donneurs doivent pouvoir prendre rendez-vous pour un don » |  
| Éviter le débordement de la salle |  OBJ-02 |  Aucune exigence justifiée |  « certains matins, la salle de prélèvement déborde » |  
| Protéger les données |  Aucun objectif défini (à valider) |  REQ-NF-01 |  « Les données doivent être protégées. » |  
  
   
   
   
   
