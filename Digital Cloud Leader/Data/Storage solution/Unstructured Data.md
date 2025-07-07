# Cloud Storage : Stockage d'objets

Cloud Storage permet de stocker des objets sous forme binaire, accompagnés de métadonnées et d'un identifiant unique (une URL). Contrairement à un système de fichiers classique, il ne repose pas sur une organisation hiérarchique, ce qui en fait un stockage **non structuré**. Il est particulièrement adapté aux **images, vidéos et enregistrements audio**.

## Classes de stockage

Cloud Storage propose plusieurs classes de stockage adaptées à différents besoins d'accès et de conservation des données :

### - Standard Storage

Convient aux données "chaudes" consultées fréquemment. Idéal pour le stockage de courte durée.

### - Nearline Storage

Conçu pour les données rarement consultées (en moyenne une fois par mois ou moins). Idéal pour des sauvegardes, des archives multimédias ou des données de longue traîne.

### - Coldline Storage

Une option économique pour les données très peu consultées (maximum une fois tous les 90 jours). Convient aux archives de long terme nécessitant un accès occasionnel.

### - Archive Storage

L'option la plus économique, idéale pour l'archivage et la reprise après sinistre. Destinée aux données accédées moins d'une fois par an. Le coût d'accès est plus élevé et la durée minimale de stockage est de **365 jours**.
Cloud Storage propose plusieurs classes de stockage adaptées à différents besoins d'accès et de conservation des données :

|Classe de stockage|Usage recommandé|Fréquence d'accès|Coût|
|---|---|---|---|
|**Standard Storage**|Données fréquemment consultées|Accès fréquent|Élevé|
|**Nearline Storage**|Données rarement consultées (1 fois par mois ou moins)|Accès occasionnel|Moyen|
|**Coldline Storage**|Données très peu consultées (1 fois tous les 90 jours)|Accès rare|Faible|
|**Archive Storage**|Données accédées moins d'une fois par an|Accès très rare|Très faible|

## Points communs entre les classes de stockage

|Caractéristique|Description|
|---|---|
|**Stockage illimité**|Aucun plafond de taille d'objet ou d'espace total.|
|**Accessibilité mondiale**|Emplacements dans plusieurs régions pour optimiser l'accès.|
|**Faible latence & haute durabilité**|Garantit une grande résilience des données.|
|**Sécurité et API unifiées**|Compatible avec les outils de sécurité et API GCP.|
|**Géoredondance**|Répartition des données sur plusieurs centres pour une protection contre les sinistres et une meilleure performance.|

## Classe de stockage automatique

Cloud Storage propose une fonctionnalité de **classe automatique**, qui optimise les coûts en déplaçant dynamiquement les objets entre différentes classes selon leur fréquence d'accès :

- Les objets rarement consultés sont transférés vers des classes "plus froides" pour **réduire les coûts**.
- Les objets fréquemment consultés sont ramenés vers le **stockage standard** pour **optimiser les performances**.
- Cette automatisation simplifie la gestion et garantit un équilibre entre **coût et performance**.