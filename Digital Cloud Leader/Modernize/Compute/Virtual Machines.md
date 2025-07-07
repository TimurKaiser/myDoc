## 1. Introduction à la Virtualisation

Par le passé, les contraintes technologiques imposaient aux entreprises de coupler des ressources matérielles spécifiques avec des applications dédiées. La virtualisation a levé ces limitations en permettant d'exécuter plusieurs systèmes sur un même matériel physique.

### Virtualisation (Virtualization)

La virtualisation est une méthode d'optimisation des ressources qui permet d'exécuter plusieurs systèmes d'exploitation sur un même serveur physique. Ces systèmes sont appelés **machines virtuelles (Virtual Machines, VM)**.

### Avantages des VM

- Exécution simultanée de plusieurs applications sur un même serveur
- Gestion et allocation des ressources simplifiées
- Réduction des coûts d'infrastructure

## 2. Compute Engine : Infrastructure as a Service (IaaS)

**Compute Engine** est un service **Infrastructure as a Service (IaaS)** de Google Cloud qui permet de créer et d'exécuter des machines virtuelles sur l'infrastructure Google. Ce service offre :

- Une tarification flexible sans investissement initial
- Une infrastructure haute performance avec des milliers de processeurs virtuels
- Des performances constantes et optimisées

## 3. Configuration des Machines Virtuelles

Les utilisateurs peuvent configurer une **instance de machine virtuelle** en définissant :

- **Processeur (CPU) et mémoire vive (RAM)**
- **Stockage (HDD/SSD)** et type d'attachement
- **Système d'exploitation (Operating System, OS)**

Les VM peuvent être créées et gérées via :
- **Google Cloud Console** (interface web de gestion des ressources Google Cloud)
- **Google Cloud CLI** (interface en ligne de commande pour automatiser la gestion)
- **Compute Engine API**
- - **Terraform** (outil d'infrastructure as code)

## 4. Facturation et Remises

### Modèle de tarification

Compute Engine facture à la seconde avec un minimum d'une minute.

### Remises disponibles

| Type de remise                                                   | Description                                                               |
| ---------------------------------------------------------------- | ------------------------------------------------------------------------- |
| **Remise pour utilisation soutenue (Sustained Use Discount)**    | Appliquée automatiquement lorsque la VM est utilisée plus de 25 % du mois |
| **Remise sur engagement d'utilisation (Committed Use Discount)** | Réduction pour un engagement d'utilisation sur 1 ou 3 ans                 |

## 5. Types de Machines Virtuelles : Spot VM et Préemptives VM

### Définition et Avantages

Les **VM Spot et Préemptives** permettent de réduire les coûts jusqu'à 90 % en exécutant des charges de travail non critiques, comme les **jobs batch** ou **analyses de données**.
Un **job batch** est un processus informatique  planifiées et exécutées à des moments précis qui exécute une série de tâches sans intervention humaine. 

### Différences entre Spot VM et Préemptive VM

| Critère               | Spot VM                         | Préemptive VM                   |
| --------------------- | ------------------------------- | ------------------------------- |
| **Durée d'exécution** | Pas de limite                   | Maximum 24 heures               |
| **Coût**              | Très réduit                     | Très réduit                     |
| **Interruption**      | Peut être arrêtée à tout moment | Peut être arrêtée à tout moment |

### Utilisation recommandée

Ces VM sont idéales pour des charges de travail **interrompables et redémarrables sans impact majeur** et tolérantes aux interruptions. 

## 6. Personnalisation des Instances

Compute Engine permet aux utilisateurs de :

- Choisir un **type de machine prédéfini** (préconfiguré par Google Cloud)
- Créer un **type de machine personnalisé** avec un nombre spécifique de **CPU et de RAM**
- Sélectionner le **système d'exploitation** et **le stockage adapté** aux besoins de l'application