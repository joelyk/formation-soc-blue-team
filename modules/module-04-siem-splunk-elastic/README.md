# Module 4 — SIEM avec Splunk/Elastic (Semaines 4-5)

Formation SOC / Blue Team | GeniusClassrooms

## Objectif

Utiliser un vrai outil SOC pour ingérer, chercher et corréler des logs.

## Sous-chapitres théoriques

- 4.1 — C'est quoi un SIEM : centraliser/corréler/alerter, Splunk vs Elastic.
- 4.2 — Architecture d'un SIEM : sources de données, index/stockage, dashboards et alertes.
- 4.3 — Requêtes Splunk (SPL) : recherche de base, `| where`, `| stats count by src_ip`, `| table`.
- 4.4 — Créer une alerte simple : condition (ex. 5 échecs de connexion en 1 min), configuration, interprétation.

## Exercices pratiques (100% local)

- Installer Splunk Free en local
- Ingérer le `auth.log` du Module 3 dans Splunk
- 5 requêtes SPL imposées par le formateur
- Tableau de bord : connexions par heure, top 5 IPs, échecs vs succès

## Projet du module — Mon premier tableau de bord SOC

Ingérer un jeu de logs (auth + réseau), créer un dashboard Splunk avec 4 visualisations pertinentes, configurer une alerte brute force, présentation orale de 5 minutes.
