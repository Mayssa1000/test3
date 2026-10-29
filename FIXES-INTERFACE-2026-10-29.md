# Correctifs interface — 29 octobre 2026

- Les marqueurs de points fixes conservent l’icône de loupe ; le style violet ne remplace plus le marqueur par un carré. Un indicateur de verrouillage signale l’état fixe.
- Les commandes principales Annuler/Rétablir sont réduites à deux flèches sans libellé ; les doublons de ruban et les commandes historiques répétées dans les barres de fenêtre sont masqués.
- L’entrée Points de contrôle est conservée dans le ruban Géoréférencement plutôt qu’en double dans Accueil.
- Le panneau Ressources reste accessible depuis l’en-tête. Le nombre de cœurs configuré est maintenant lu par la génération des tuiles de géoréférencement (plafond de sécurité : 8 workers). Le budget RAM est volontairement présenté comme indicatif, car il ne constitue pas une limite mémoire système stricte.
- La landing page charge `/worldLow-pixel-map.html` dans une iframe de fond interactive, sous la carte de présentation. Placez ce fichier dans `static/worldLow-pixel-map.html` avant déploiement. Le fichier de fond n’est pas inclus dans cette archive car il n’a pas été fourni ici.
- Le logo d’en-tête garde une taille indépendante du logo de landing page et le marqueur fixe conserve ses images de fond.

Vérifications effectuées : syntaxe JavaScript des scripts intégrés (`node --check`). Aucun test de navigateur interactif complet n’a été exécuté.

## Ajustements supplémentaires du ruban et des marqueurs
- Accueil limité à Ouvrir image(s), Ouvrir projet et Enregistrer.
- Fusionner les images n'est proposé qu'une fois dans l'onglet Image.
- Géoréférencement utilise le sélecteur de méthode unique (Affine par défaut) et Points de contrôle, sans second bouton Affine.
- L'onglet Carte présente Fonds de carte et Vue globe; la commande Mesure & dessin reste dans la fenêtre Carte.
- Le contrôle 3D principal reste dans la fenêtre Carte; le doublon de l'ancien panneau Outils est masqué.
- Ajout des ressources statiques loupe.svg et world.svg pour éviter les références à des SVG absents.
- Icône de point agrandie et style du point fixé forcé à conserver l'icône plutôt qu'un carré coloré.
- Taille du logo de l'en-tête verrouillée à 32 px même lors du changement de thème; la taille configurable du logo de landing page reste indépendante.
