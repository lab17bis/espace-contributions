# Journal des modifications

Les fichiers publiés ne sont jamais retirés : chaque version ajoute ou corrige, sans casser l'existant.

## 2026-11-26 (questionnaire et vote public)

### Modifié
- Documentation : le widget grist-questionnaire sait maintenant classer par ordre (glisser-déposer), proposer un tableau de choix, un choix « Autre », des bornes de choix, une réponse par défaut, un ordre aléatoire, des types lien, heure et date et heure, et intégrer image, son, vidéo et PDF. Ces options sont facultatives et déjà disponibles dans cet espace (le widget est lu à l'adresse stable `/v1/`). Le vote public a désormais cinq niveaux d'identification au choix par consultation (ouvert, courriel déclaré, code commun, code individuel, compte Grist) ; un document déjà installé se met à jour d'un clic dans les réglages. Aucun changement dans les fichiers `.grist`.

## 2026-11-26

### Modifié
- Documentation : les deux façons de voter (identifié dans Grist, public par code), ce que montre la page publique, et l'affichage d'une page sans menus Grist. Aucun changement dans les fichiers `.grist`.

## 2026-11-24

### Modifié
- Documentation : l'outil de consultation s'appelle désormais `grist-consultation` (ancien nom `grist-decision`).
- Les fichiers `.grist` à importer pointent vers `lab17bis.github.io/grist-consultation/v1/` (ancienne adresse `grist-decision`), images d'exemple comprises.
- Les nouvelles tables Consultations reçoivent la colonne `Config_consultation` (les documents existants gardent `Config_decision`, toujours lue).
