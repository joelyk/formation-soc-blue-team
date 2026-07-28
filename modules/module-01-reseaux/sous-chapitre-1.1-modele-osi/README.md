# Chapitre 1 — Le modèle OSI

Module 1 — Les réseaux et protocoles | Formation Blue Team | GeniusClassrooms

## Résumé

Le modèle **OSI** (Open Systems Interconnection, ISO, 1984) découpe la communication réseau en **7 couches**, chacune ayant une responsabilité unique. Pour un analyste Blue Team, ce modèle est une carte mentale : chaque type d'attaque cible une couche précise, ce qui permet de savoir immédiatement où chercher dans les logs et quel outil utiliser.

| # | Couche | Rôle principal | Protocoles clés | Attaques associées |
|---|--------|-----------------|------------------|----------------------|
| 7 | Application | Interface utilisateur | HTTP, DNS, SMTP, FTP | Phishing, SQLi, DDoS L7 |
| 6 | Présentation | Format et chiffrement | TLS, SSL | Downgrade TLS, faux certificats |
| 5 | Session | Gestion des sessions | NetBIOS, RPC | Session Hijacking |
| 4 | Transport | Ports et fiabilité | TCP, UDP | SYN Flood, scan de ports |
| 3 | Réseau | Routage entre réseaux | IP, ICMP | IP Spoofing, DDoS volumétrique |
| 2 | Liaison | Communication locale | Ethernet, ARP, MAC | ARP Poisoning, MAC Flooding |
| 1 | Physique | Signal brut | Câble, Wi-Fi, fibre | Wiretapping, débranchement |

**Réflexe SOC** : face à une alerte, se demander *à quelle couche* se situe l'anomalie (ex. flood de SYN → couche 4 ; requêtes DNS vers domaines aléatoires → couche 7 / DNS Tunneling ou C2 ; TLS 1.0 détecté → couche 6).

## Exercice théorique — identifier la couche d'une attaque

Associer 5 scénarios (flood HTTP, cache ARP corrompu, DNS tunneling, session bancaire détournée, TLS 1.0 en prod) à leur couche OSI.

➡️ Réponses et notes personnelles : [`exercice-theorique.md`](exercice-theorique.md)

## Exercice pratique — observer l'OSI en temps réel avec Wireshark

Capturer son propre trafic réseau (navigation web, 30 s), puis via **Statistics > Protocol Hierarchy**, relever les protocoles observés par couche (Ethernet/L2, IP/L3, TCP-UDP/L4, HTTP-DNS-TLS/L7) et évaluer leur normalité.

Cette capture constitue la première brique du rapport d'analyse réseau final du module.

➡️ Capture et notes : [`exercice-pratique/`](exercice-pratique/)

## Ressources

- Wireshark : https://www.wireshark.org
