
**Données Semi-Structurées**

Les **données semi-structurées** sont un mélange entre des données structurées et non structurées. Elles ne suivent pas une organisation rigide comme dans les bases de données relationnelles, mais elles possèdent certains éléments cohérents (par exemple, des tags ou des clés).

**Exemple :** Un e-mail, bien qu’il contienne du texte libre (données non structurées), comporte également des éléments réguliers comme l’adresse de l’expéditeur, la date et l’objet (données semi-structurées).


## **Firestore 

Firestore est une base de données NoSQL, flexible et évolutive. Elle permet de stocker et de synchroniser des données en temps réel, idéale pour les applications mobiles et Web.

#### **Caractéristiques principales :**

| **Caractéristique**      | **Détails**                                                          |
| ------------------------ | -------------------------------------------------------------------- |
| **Type**                 | NoSQL (Non-Relational Database)                                      |
| **Stockage des données** | Documents (objets imbriqués (JSON, XML...), chiffres, chaînes, etc.) |
| **Organisation**         | Stockage en **collections** de **documents**                         |
| **Évolutivité**          | **Scaling automatique**, gestion de la charge utilisateur            |
| **Accès hors ligne**     | Synchronisation des données en mode hors ligne                       |
| **Synchronisation**      | En temps réel (idéal pour des apps mobiles)                          |
 
 #### **Avantages de Firestore :**

- **Evolutivité horizontale** : Adapté aux applications à grande échelle avec une montée en charge fluide.
- **Synchronisation en temps réel** : Mises à jour instantanées des données sur tous les appareils connectés.
- **Stockage flexible** : Support des types de données variés avec une structure dynamique.
- **Automatique** : S'adapte automatiquement à la demande pour garantir des performances constantes, quelle que soit la taille de la base de données.


## **Cloud Bigtable**

**Base de données Big Data NoSQL**

Cloud Bigtable est un service NoSQL conçu pour des cas d'utilisation à grande échelle, traitant des données volumineuses, avec des exigences de faible latence et de débit élevé. Idéal pour les applications d’analyse en temps réel ou les séries temporelles.

#### **Caractéristiques principales :**

| **Caractéristique**   | **Détails**                                                                                          |
| --------------------- | ---------------------------------------------------------------------------------------------------- |
| **Type**              | NoSQL Big Data                                                                                       |
| **Cas d'utilisation** | IoT, analyses utilisateur, données financières, séries temporelles (séquence de donné chronologique) |
| **Débit et Latence**  | **Faible latence** et **haut débit** pour traiter de grandes quantités de données                    |
| **Volume de données** | Conçu pour des volumes supérieurs à 1 To de données structurées/semi-structurées                     |
| **Évolutivité**       | Haute évolutivité horizontale (ajustement automatique aux besoins)                                   |

#### **Cas d’utilisation typiques de Cloud Bigtable :**

- **IoT (Internet des Objets)** : Pour stocker et analyser les données de capteurs en temps réel.
- **Données financières** : Stockage et traitement des transactions financières en grande quantité.
- **Machine Learning** : Utilisation des données pour entraîner des modèles d'IA et de machine learning.

---

### **Quand choisir Firestore ou Cloud Bigtable ?**

| **Critère**           | **Firestore**                                               | **Cloud Bigtable**                                           |
| --------------------- | ----------------------------------------------------------- | ------------------------------------------------------------ |
| **Type de données**   | Semi-structurées ou non structurées                         | Structurées, semi-structurées ou séries temporelles          |
| **Cas d’usage**       | Applications mobiles/Web, synchronisation en temps réel     | Big Data, analyse temps réel, séries temporelles             |
| **Évolutivité**       | Auto-scaling flexible pour petites et moyennes applications | Haute évolutivité pour très grandes charges de travail       |
| **Volume de données** | Moins de 1 To                                               | Plus de 1 To                                                 |
| **Latence et débit**  | Faible latence pour des données à petite échelle            | Faible latence et haut débit pour de gros volumes de données |

---

### **Résumé**

- **Firestore** est idéal pour les applications nécessitant une gestion en temps réel, de petites à moyennes quantités de données semi-structurées et une synchronisation hors ligne.
- **Cloud Bigtable** excelle dans le traitement de grandes quantités de données à faible latence et haut débit, comme les séries temporelles ou les données IoT.

Cloud Bigtable est un service NoSQL conçu pour des cas d'utilisation à grande échelle, traitant des données volumineuses, avec des exigences de faible latence et de débit élevé. Idéal pour les applications d’analyse en temps réel ou les séries temporelles.


