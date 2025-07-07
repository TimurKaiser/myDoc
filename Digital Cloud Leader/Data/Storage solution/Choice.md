# Unstructured Data

Pour les données non structurées, l'option la plus viable reste **Cloud Storage**. Il est nécessaire de choisir une classe en fonction du taux d'utilisation des données. L'**Autoclass** permettra ensuite de déterminer la classe appropriée pour chaque donnée en fonction de son usage.

![[Unstructured Choice.png]]


# Structured and Semi-Structured Data

Le choix se complique davantage lorsqu'il s'agit de choisir une solution de stockage pour les **données structurées** ou **semi-structurées**. Le choix se fait en fonction de la **nature des données** et des **besoins du business**.

Si vous disposez de données structurées ou semi-structurées, votre choix dépendra de la **nature de vos charges de travail** : **transactionnelles** ou **analytiques**.

1. **Charges de travail transactionnelles (Transactional Workload)** :
    
    - Ces charges proviennent des **systèmes de gestion des transactions en ligne** (OLTP - Online Transaction Processing). Ce type de travail est utilisé lorsqu'il est nécessaire de **mettre à jour ou insérer des données rapidement**, souvent en temps réel.
    - Ces systèmes se concentrent sur les **opérations rapides** telles que l'ajout de nouveaux enregistrements ou la modification de données existantes. Ce sont des systèmes où chaque transaction doit être exécutée de manière fiable et rapide, avec peu de latence.
    - **Exemple** : Un site de commerce électronique qui enregistre chaque achat immédiatement dans une base de données.
2. **Charges de travail analytiques (Analytical Workload)** :
    
    - Ces charges proviennent des **systèmes de traitement analytique en ligne** (OLAP - Online Analytical Processing). Elles sont utilisées lorsqu'il faut **analyser de grandes quantités de données**, souvent pour des rapports ou des analyses approfondies.
    - Ces systèmes sont conçus pour effectuer des **requêtes complexes** et **agrégations** sur de grands ensembles de données, comme les calculs de moyennes, de sommes, ou d’autres types d’analyses sur des séries temporelles.
    - **Exemple** : Analyser les données historiques de ventes pour comprendre les tendances à long terme ou produire des rapports d'analyse financière.- 


![[SrtucOrSemi Choice.png]]