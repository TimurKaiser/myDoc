# Observabilité sur Google Cloud Platform (GCP)

## Introduction

L'observabilité (Observability) dans le cloud consiste à collecter, analyser et visualiser des données afin d'obtenir des insights sur les performances, l'état et le comportement des systèmes. Contrairement aux environnements sur site, il n'est pas possible d'accéder physiquement aux serveurs dans le cloud.

Pour répondre à ce besoin, Google Cloud propose **la suite Operations**, une plate-forme unifiée de surveillance, journalisation et diagnostic permettant de gérer et d'optimiser les performances et la disponibilité des applications et de l'infrastructure.
![[Op.png]]
## Services de la suite Operations

| Service              | Description                                                                                                                                                                                                                                                               |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Cloud Monitoring** | Collecte des mesures, journaux et traces pour fournir des insights sur l'état, les performances et la disponibilité de l'infrastructure et des applications. Il permet de définir des règles d'alerte basées sur des métriques et des vérifications de disponibilité.     |
| **Cloud Logging**    | Collecte et stocke les journaux d'application et d'infrastructure. Il offre des insights en temps réel pour le débogage, l'analyse des tendances et la conformité réglementaire.                                                                                          |
| **Cloud Trace**      | Identifie les goulots d'étranglement des applications en collectant les données de latence et en fournissant des insights sur les performances.                                                                                                                           |
| **Cloud Profiler**   | Analyse l'utilisation des ressources (CPU, mémoire) en production pour optimiser les performances des applications.                                                                                                                                                       |
| **Error Reporting**  | Détecte, analyse et regroupe en temps réel les erreurs applicatives. Il présente une interface centralisée avec tri, filtrage et affichage détaillé des erreurs (occurrences, impact utilisateur, traces d'exception). Il permet l'envoi d'alertes par e-mail et via API. |

## Conclusion

Les outils d'observabilité intégrés à la suite Operations de Google Cloud offrent une visibilité complète sur les performances et l'état des applications et de l'infrastructure cloud, permettant ainsi une gestion optimisée et réactive des systèmes en production.