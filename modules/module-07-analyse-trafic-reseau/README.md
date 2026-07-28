# Module 7 — Analyse de Trafic Réseau (Semaine 8)

Formation SOC / Blue Team | GeniusClassrooms

## Objectif

Lire des captures réseau et détecter des comportements malveillants.

## Sous-chapitres théoriques

- 7.1 — Rappels Wireshark : interface, filtres essentiels (`tcp`, `http`, `dns`, `ip.addr == x.x.x.x`), suivi de flux TCP.
- 7.2 — Signatures d'attaques dans le trafic : scan Nmap, beacon C2, exfiltration de données.
- 7.3 — Analyser un fichier PCAP : vue d'ensemble puis zoom, statistiques Wireshark, extraction de fichiers transférés.
- 7.4 — Rédiger un rapport d'analyse réseau : contexte, observations, conclusions, IOCs.

## Exercices pratiques (100% local)

- Fichiers `.pcap` fournis par le formateur
- Trouver le scan Nmap dans un pcap
- Identifier l'IP qui exfiltre des données
- Reconstituer un téléchargement HTTP depuis un pcap

## Projet du module — PCAP d'incident

À partir d'un `.pcap` simulant un incident complet (scan + exploitation + exfiltration) : reconstruire la chronologie de l'attaque, identifier toutes les IPs impliquées, extraire les IOCs réseau, rédiger un rapport d'incident de 2-3 pages.
