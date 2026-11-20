# espace-contributions

> **Espace Grist clé en main.** Un document Grist prêt à l'emploi pour **faire participer une équipe ou un service** : une boîte à idées, un mur des réalisations dont les équipes sont fières, des consultations pour prioriser ou choisir, et la suite donnée à chaque proposition, au Système de design de l'État (DSFR).

Un **espace** est un document Grist complet — tables, formules, pages, widgets et réglages — à importer en une fois. Il assemble des widgets de la famille `grist-…` autour d'une manière de travailler. Chaque widget reste utilisable seul.

## À quoi ça sert

- **Recueillir des idées** à tout moment, des personnes connectées au document comme de celles qui n'y ont pas accès (formulaire public).
- **Valoriser des réalisations** : chaque équipe partage ce dont elle est fière, avec une image et un lien ; les collègues la soutiennent.
- **Prioriser ou choisir** : vote par points, choix unique ou notation selon des critères pondérés, avec des résultats cachés jusqu'à la clôture si besoin.
- **Répondre** : chaque proposition reçoit une suite visible (à l'étude, retenue, en cours, réalisée, non retenue) et une explication.
- **Rendre compte** : participation, propositions par mois, suites données, propositions en attente de réponse depuis plus d'un mois.

## Ce que contient l'espace

| Page | Outil | Contenu |
| --- | --- | --- |
| **Consultations** | [grist-decision](https://github.com/lab17bis/grist-decision) | Consultations en cours et closes, mur des propositions, dépôt, vote, résultats et suites. Tables `Consultations`, `Propositions`, `Criteres`, `Votes`, `Votants`. |
| **Formulaire de dépôt** | [grist-questionnaire](https://github.com/lab17bis/grist-questionnaire) | Formulaire public pour déposer une proposition sans accès au document. Les propositions arrivent dans la consultation cochée « Reçoit le formulaire public ». |
| **Indicateurs** | [grist-graphique](https://github.com/lab17bis/grist-graphique) | Participation et suites données. Page *Régler les indicateurs* pour le modifier. |
| **Propositions** | tables Grist | Toutes les propositions et leurs soutiens ; page *Votes* pour le détail. Cochez *Masquée* pour retirer un doublon. |

## L'installer en 2 minutes

1. **Télécharger** le fichier de l'espace :
   - [`espace-contributions.grist`](https://github.com/lab17bis/espace-contributions/raw/main/espace-contributions.grist) : l'espace vide, prêt à l'usage ;
   - [`espace-contributions-exemple.grist`](https://github.com/lab17bis/espace-contributions/raw/main/espace-contributions-exemple.grist) : le même, rempli de données fictives, pour essayer.
2. **L'importer dans Grist** : depuis l'accueil de votre espace Grist, *Ajouter › Importer un document*, puis choisissez le fichier.
3. **L'ouvrir** : les pages et les widgets sont déjà en place. Si Grist le demande, confirmez l'accès complet des widgets au document.
4. **Inviter l'équipe** (*Partager*), en éditeur pour celles et ceux qui saisissent.

Vous êtes propriétaire du document importé. Rien n'est installé ailleurs : les widgets sont des pages web publiques, qui lisent et écrivent dans votre document avec les droits de la personne connectée.

Les widgets sont chargés depuis leur **adresse stable** (`…/v1/`) : une évolution d'un widget ne modifie pas votre espace sans que vous l'ayez décidé.

## Le régler

- **Consultations** : bouton *Nouvelle consultation*, puis onglet *Gérer* de chaque consultation (mode de vote, étape, échéance, visibilité des résultats, critères). Lien *Réglages* en bas du widget pour les types de propositions et les suites possibles.
- **Formulaire public** : page *Formulaire de dépôt*, puis onglet *Publication* pour obtenir le lien. Cochez *Reçoit le formulaire public* sur une seule consultation.
- **Indicateurs** : page *Régler les indicateurs*.

Les réglages sont enregistrés dans le document. Ils partagent les mêmes réglages d'en-tête et de pied de page.

## Données et droits d'accès

Pour déposer et voter, les personnes doivent être invitées **en éditeur**. Les votes portent l'adresse de leur auteur : ils ne sont pas anonymes pour les propriétaires du document, qui voient la table `Votes`. Pour les masquer, ajoutez une règle d'accès sur cette table dans *Permissions avancées*. C'est un outil de consultation, pas de scrutin. Le formulaire public permet seulement **d'ajouter** une proposition.

Les tables `Personnes` et `Structures`, quand l'espace en contient, suivent la règle commune des widgets : un widget de la famille ajouté plus tard les reprend et les complète, au lieu d'en créer d'autres.

Les fichiers de ce dépôt ne contiennent aucune donnée réelle. L'exemple est entièrement fictif.

## Widgets utilisés

- [grist-questionnaire](https://github.com/lab17bis/grist-questionnaire) : questionnaires au DSFR avec logique conditionnelle et notes sur une échelle.
- [grist-graphique](https://github.com/lab17bis/grist-graphique) : tableaux de bord et indicateurs à seuils au DSFR.
- [grist-decision](https://github.com/lab17bis/grist-decision) : consultations : boîte à idées, valorisation des réalisations, votes et suites données.

## Autres espaces

- [espace-pilotage](https://github.com/lab17bis/espace-pilotage) : regarder et décider : un écran d'équipe qui rassemble indicateurs, réunions, projets, priorités et parties prenantes.
- [espace-collaboratif](https://github.com/lab17bis/espace-collaboratif) : faire ensemble : réunions, projets partagés, décisions collectives et ressources communes d'une équipe.
- [espace-accompagnement](https://github.com/lab17bis/espace-accompagnement) : suivre les personnes qui sollicitent un service : offre de service, sollicitations, fiches contact et satisfaction.
- [espace-sondage](https://github.com/lab17bis/espace-sondage) : concevoir un questionnaire, savoir qui a répondu et lire les résultats en indicateurs.
- [espace-reseau](https://github.com/lab17bis/espace-reseau) : animer un réseau ou une communauté de pratique : membres, groupes, rencontres, présences, ressources partagées, retours, carte et liens entre acteurs.

## Écosystème

- **[Grist](https://grist.numerique.gouv.fr)** : tableur-base de données libre ([gristlabs/grist-core](https://github.com/gristlabs/grist-core)), proposé aux agents publics par la [DINUM](https://www.numerique.gouv.fr/) dans [La Suite numérique](https://lasuite.numerique.gouv.fr/). L'espace s'importe dans toute instance de Grist.
- **[Système de design de l'État (DSFR)](https://www.systeme-de-design.gouv.fr/)** ([GouvernementFR/dsfr](https://github.com/GouvernementFR/dsfr)). Son usage est réservé aux sites des services de l'État.

## Mots-clés

Grist, espace Grist, modèle Grist, document clé en main, boîte à idées, innovation participative, valorisation, réalisations, fierté, consultation, vote, vote par points, priorisation, budget participatif, suites données, DSFR, Système de design de l'État, La Suite numérique, service public, logiciel libre.

## Licence

Fichiers de l'espace et documentation sous licence Creative Commons [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.fr) : réutilisation et adaptation autorisées, en citant la source et en partageant sous la même licence. Le code des widgets est sous licence MIT, dans leurs dépôts.

Conçu par le Lab 17 bis, laboratoire d'innovation publique de l'académie de Reims. Contact : <lab17bis@ac-reims.fr>
