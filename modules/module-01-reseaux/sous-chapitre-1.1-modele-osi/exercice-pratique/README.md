# Exercice pratique — Observer l'OSI en temps réel avec Wireshark

## Protocole

1. Lancer Wireshark, sélectionner l'interface active, démarrer la capture.
2. Naviguer sur 2-3 sites web pendant ~30 secondes.
3. Arrêter la capture.
4. `Statistics > Protocol Hierarchy` pour lister les protocoles par couche.

## Relevé par couche

| Couche | Protocole observé | Rôle | Normal / Suspect ? |
|--------|--------------------|------|----------------------|
| 2 — Liaison | Ethernet | | |
| 3 — Réseau | IP | | |
| 4 — Transport | TCP / UDP | | |
| 7 — Application | HTTP / DNS / TLS | | |

## Fichier de capture

Placer le `.pcapng` généré dans ce dossier (ex. `capture-chapitre-01.pcapng`). Il sert de base au rapport d'analyse réseau final du module.

> Note : les fichiers `.pcap`/`.pcapng` sont ignorés par git (voir `.gitignore`) car volumineux — à partager séparément si besoin pour la formation.
