# Exercice 5 — Reconnaître un scan de ports

Lié à : Chapitre 5 — Firewall, IDS, IPS et DMZ

## Consigne

À partir d'un fichier `.pcap` fourni (ou d'une capture Wireshark), repérer la signature d'un scan de ports : nombreuses connexions vers des ports différents sur une même IP, en un temps très court, souvent sans finalisation du handshake TCP (paquets SYN sans ACK final).

## Relevé

| Champ | Valeur |
|-------|--------|
| IP source (scanner présumé) | |
| IP cible | |
| Nombre de ports testés | |
| Durée du scan | |
| Type de scan supposé (SYN scan, connect scan...) | |

## Question

Quelle règle de firewall ou quelle alerte IDS permettrait de détecter/bloquer ce comportement ?

**Réponse :**
