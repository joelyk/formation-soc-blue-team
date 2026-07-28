# Module 1 — Les réseaux (Semaines 1-2)

Formation SOC / Blue Team | GeniusClassrooms

## Objectif

Comprendre comment les données circulent sur un réseau — base indispensable pour analyser des attaques.

## Sous-chapitres théoriques

- [1.1 — Le modèle OSI](sous-chapitre-1.1-modele-osi/README.md) : rôle de chaque couche, mapping attaques/couches.
- 1.2 — TCP/IP en pratique : TCP vs UDP, 3-way handshake, pourquoi c'est important en cybersécurité.
- 1.3 — Les protocoles essentiels : DNS, HTTP vs HTTPS, DHCP, ARP.
- 1.4 — Adressage IP et sous-réseaux : IPv4, masques, CIDR, IP privées/publiques, ports importants (22, 80, 443, 445, 3389).

## Exercices pratiques (100% local)

- Installer Wireshark et capturer son propre trafic réseau
- `ping`, `traceroute`, `netstat -an` : lancer et analyser les résultats
- Identifier dans Wireshark un handshake TCP, une requête DNS, une requête HTTP
- Exercice papier : dessiner le chemin d'un paquet du PC jusqu'à google.com, couche par couche

## Projet du module — Cartographie réseau de ma machine

Capturer 10 minutes de trafic réseau avec Wireshark, identifier les 5 protocoles les plus présents, repérer les IPs contactées, et rédiger un rapport d'une page.
