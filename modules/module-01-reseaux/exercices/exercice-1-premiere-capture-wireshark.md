# Exercice 1 — Première capture Wireshark

Lié à : [Chapitre 1 — Le modèle OSI](../chapitre-01-modele-osi/README.md)

## Consigne

1. Installer Wireshark, sélectionner l'interface réseau active.
2. Démarrer la capture, naviguer sur 2-3 sites web pendant ~30 secondes, arrêter la capture.
3. `Statistics > Protocol Hierarchy` : relever les protocoles présents par couche OSI.

## Relevé

| Couche | Protocole observé | Rôle | Normal / Suspect ? |
|--------|--------------------|------|----------------------|
| 2 — Liaison | Ethernet | | |
| 3 — Réseau | IP | | |
| 4 — Transport | TCP / UDP | | |
| 7 — Application | HTTP / DNS / TLS | | |

## Fichier de capture

Placer le `.pcapng` généré ici ou dans un dossier `captures/` (ignoré par git, voir `.gitignore`). Sert de base au projet du module.
