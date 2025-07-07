

**Dataflow** est un service qui permet de créer des **pipelines de données** pour le traitement des données en temps réel (flux) ou en batch (lot). Ces pipelines permettent d'exécuter des tâches ETL (Extraction, Transformation, Chargement) sur les données, ce qui inclut des étapes d'extraction, de transformation et de chargement des données dans des systèmes de stockage ou d'analyse.
- **Pipelines de données** : Un pipeline Dataflow représente une série d'étapes qui ingèrent des données brutes et les déplacent vers une destination de stockage, telle qu'un entrepôt de données.
- **Traitement des données** : Dataflow gère le traitement des données en temps réel ou par lot, permettant de collecter, transformer et analyser les données de manière cohérente.

### **Caractéristiques clés de Dataflow** :

- **Infrastructure entièrement gérée et sans serveur** : Dataflow est un service entièrement géré et sans serveur. Cela signifie que vous n'avez pas à vous soucier du provisionnement ou de la gestion des ressources pour exécuter les pipelines. Dataflow gère automatiquement l'infrastructure et le dimensionnement des ressources.
- **Autoscaling** : Le service ajuste automatiquement les ressources en fonction des besoins du pipeline, garantissant une **réactivité fiable** et une gestion optimisée des ressources.
- **Simplification des tâches opérationnelles** : En étant un service sans serveur et entièrement géré, Dataflow permet aux utilisateurs de se concentrer sur l'analyse des données plutôt que sur la gestion des ressources ou de l'infrastructure.


**Dataflow** crée donc des **pipelines de données**, qui sont une série d'étapes à suivre pour traiter des données. Ces données peuvent être issues de flux en temps réel ou de lots envoyés par **Pub/Sub**. Lorsque **Pub/Sub** envoie un message ou un événement, **Dataflow** peut déclencher un pipeline de traitement pour effectuer des opérations telles que l'extraction, la transformation et le chargement (ETL) des données, afin de les préparer pour l'analyse ou de les stocker dans une destination finale (par exemple, BigQuery).