# KalipheTiles — UX/UI compact et modes carte

## Changements
- Ruban de travail conservé, avec panneaux de commandes plus compacts et hiérarchie visuelle inspirée d'Office.
- Paramètres généraux structurés en sections repliables : « Général · Points de contrôle » et « Options · Dessin et mesure ».
- Ajout d'un sélecteur de mode permanent dans la fenêtre Carte : « Géoréférencer » ou « Mesurer & dessiner ».
- En mode Géoréférencer, un clic carte place un point de contrôle et la barre de dessin est masquée par défaut.
- En mode Mesurer & dessiner, les outils de dessin/mesure sont affichés. Le clic sur la carte ne place plus accidentellement de point de contrôle.
- Le bouton Outils permet de masquer/afficher manuellement les outils cartographiques.
- Ctrl+Z / Ctrl+Y dans la fenêtre Carte sont routés selon le mode actif : historique GCP en géoréférencement, historique des dessins/mesures en mode dessin.
- Landing page et logo existants préservés.

## Validation
- Syntaxe JavaScript vérifiée avec Node.js.
- Modules Python compilés avec `py_compile`.
- Pas de test E2E dans un navigateur interactif réalisé pour cette archive.

## Limites
- L'historique carte porte sur les mesures/dessins existants ; il ne constitue pas un historique complet de chaque modification des fonds de carte ou de la navigation.
- Les raccourcis ne détournent pas la saisie lorsque le focus est dans un champ de formulaire.
