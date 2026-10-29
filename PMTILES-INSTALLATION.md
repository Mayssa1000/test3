# Installation automatique de PMTiles

KalipheTiles peut installer le CLI officiel PMTiles à la demande : menu **Fichier → Installer PMTiles**. L'export PMTiles lance aussi cette installation si le CLI est absent.

Le programme télécharge la dernière release de `protomaps/go-pmtiles` depuis l'API GitHub officielle, choisit l'archive correspondant au système et à l'architecture, extrait uniquement le binaire `pmtiles`/`pmtiles.exe`, puis vérifie son exécution avec `pmtiles version`.

Le binaire est installé dans `~/.kaliphetiles/bin`. L'installation requiert une connexion Internet et l'accès à GitHub. Aucun privilège administrateur n'est demandé. Si le réseau est bloqué ou si aucune release compatible n'est publiée, le message d'erreur fournit le lien officiel : https://github.com/protomaps/go-pmtiles/releases.

Documentation officielle : https://docs.protomaps.com/pmtiles/cli
