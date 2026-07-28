# Module 3 — Analyse de logs (Semaines 3-4)

Formation SOC / Blue Team | GeniusClassrooms

## Objectif

Savoir lire des logs comme un analyste SOC et détecter une activité suspecte.

## Sous-chapitres théoriques

- 3.1 — Types de logs : authentification, réseau, applicatifs ; différences Windows/Linux.
- 3.2 — Event IDs Windows critiques : 4624 (connexion réussie), 4625 (échec), 4688 (nouveau processus), 4720 (création compte), 4732 (ajout à un groupe privilégié).
- 3.3 — Lire un log comme un analyste : qui/quand/depuis où/quoi, repérer les anomalies, corrélation.
- 3.4 — Premiers IOC (Indicator of Compromise) : IP malveillante, hash suspect, domaine bizarre.

## Exercices pratiques (100% local)

- Générer ses propres logs (fausses tentatives de connexion sur la VM)
- Fichiers `.log` d'exemple fournis par le formateur
- Trouver 3 tentatives de brute force cachées dans un `auth.log` de 500 lignes
- Windows : filtrer l'Observateur d'événements par Event ID 4625

## Projet du module — Détective de logs

Analyse d'un `auth.log` fictif contenant une attaque simulée (brute force + connexion suspecte réussie) : identifier l'IP attaquante, l'heure, le compte ciblé, le succès ou non de l'attaque, et rédiger un rapport d'incident d'une page.
