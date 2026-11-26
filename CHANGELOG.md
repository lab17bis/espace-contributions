# Journal des modifications

Les fichiers publiés ne sont jamais retirés : chaque version ajoute ou corrige, sans casser l'existant.

## 2026-11-26

### Modifié
- Documentation : les deux façons de voter (identifié dans Grist, public par code), ce que montre la page publique, et l'affichage d'une page sans menus Grist. Aucun changement dans les fichiers `.grist`.

## 2026-11-24

### Modifié
- Documentation : l'outil de consultation s'appelle désormais `grist-consultation` (ancien nom `grist-decision`).
- Les fichiers `.grist` à importer pointent vers `lab17bis.github.io/grist-consultation/v1/` (ancienne adresse `grist-decision`), images d'exemple comprises.
- Les nouvelles tables Consultations reçoivent la colonne `Config_consultation` (les documents existants gardent `Config_decision`, toujours lue).
