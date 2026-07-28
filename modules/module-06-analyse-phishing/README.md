# Module 6 — Analyse de Phishing (Semaine 7)

Formation SOC / Blue Team | GeniusClassrooms

## Objectif

Savoir analyser un email malveillant de A à Z comme un analyste Tier 1.

## Sous-chapitres théoriques

- 6.1 — Anatomie d'un email : headers (`From`, `Reply-To`, `Received`, `X-Originating-IP`), expéditeur affiché vs réel.
- 6.2 — Techniques de phishing : spoofing de domaine, homoglyphes, urgence/manipulation, pièces jointes vs liens malveillants.
- 6.3 — Analyse d'une URL suspecte : décomposition, redirections, URLScan.io, VirusTotal.
- 6.4 — Processus d'investigation : headers → liens → pièces jointes (sandbox) → documentation/escalade.

## Exercices pratiques (100% local ou très léger)

- 5 exemples d'emails phishing fictifs (`.eml`) fournis par le formateur
- Extraction et lecture des headers
- Identifier technique, objectif et IOCs par email
- Fiche d'analyse standardisée par email

## Projet du module — Campagne phishing : investigation complète

Analyser 3 emails suspects signalés par des employés, remplir une fiche d'incident par email, déterminer la malveillance et le lien entre campagnes, rédiger un rapport de synthèse avec recommandations.
