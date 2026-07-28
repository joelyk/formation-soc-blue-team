# Module 2 — Linux & Administration système (Semaines 2-3)

Formation SOC / Blue Team | GeniusClassrooms

## Objectif

Maîtriser l'environnement Linux, cœur des outils SOC.

## Sous-chapitres théoriques

- 2.1 — Structure du système : arborescence (`/etc`, `/var/log`, `/home`, `/tmp`, `/proc`) et criticité en sécurité.
- 2.2 — Commandes essentielles : navigation (`ls`, `cd`, `find`, `locate`), lecture (`cat`, `less`, `grep`, `tail -f`), processus (`ps aux`, `top`, `kill`), réseau (`ss -tulnp`, `ip a`, `netstat`).
- 2.3 — Permissions et utilisateurs : `chmod`, `chown`, rwx, utilisateurs/groupes/`sudo`, risques liés aux permissions mal configurées.
- 2.4 — Logs système : `/var/log/auth.log`, `/var/log/syslog`, `/var/log/kern.log`, recherche avec `grep`.

## Exercices pratiques (100% local)

- Installer Ubuntu ou Kali Linux en VM (VirtualBox)
- 20 commandes imposées par le formateur
- Trouver les fichiers modifiés dans les dernières 24h (`find`)
- Lire `/var/log/auth.log` : connexions réussies vs échouées

## Projet du module — Audit basique d'un système Linux

Lister les utilisateurs, vérifier les permissions des fichiers sensibles (`/etc/passwd`, `/etc/shadow`), consulter les 50 dernières lignes de `auth.log`, produire un mini-rapport sur la configuration du système.
