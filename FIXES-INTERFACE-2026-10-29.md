# Correctifs interface — 29 octobre 2026

- Les marqueurs de points fixes conservent l’icône de loupe ; le style violet ne remplace plus le marqueur par un carré. Un indicateur de verrouillage signale l’état fixe.
- Les commandes principales Annuler/Rétablir sont réduites à deux flèches sans libellé ; les doublons de ruban et les commandes historiques répétées dans les barres de fenêtre sont masqués.
- L’entrée Points de contrôle est conservée dans le ruban Géoréférencement plutôt qu’en double dans Accueil.
- Le panneau Ressources reste accessible depuis l’en-tête. Le nombre de cœurs configuré est maintenant lu par la génération des tuiles de géoréférencement (plafond de sécurité : 8 workers). Le budget RAM est volontairement présenté comme indicatif, car il ne constitue pas une limite mémoire système stricte.
- La landing page charge `/worldLow-pixel-map.html` dans une iframe de fond interactive, sous la carte de présentation. Placez ce fichier dans `static/worldLow-pixel-map.html` avant déploiement. Le fichier de fond n’est pas inclus dans cette archive car il n’a pas été fourni ici.
- Le logo d’en-tête garde une taille indépendante du logo de landing page et le marqueur fixe conserve ses images de fond.

Vérifications effectuées : syntaxe JavaScript des scripts intégrés (`node --check`). Aucun test de navigateur interactif complet n’a été exécuté.
