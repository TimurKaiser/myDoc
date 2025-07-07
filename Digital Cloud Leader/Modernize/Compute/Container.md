### Conteneurs vs Machines Virtuelles (VM)

Les **conteneurs** (containers) et les **machines virtuelles** (VMs) offrent des environnements isolés pour exécuter des services, mais les **conteneurs** sont plus efficaces.

- **VMs** virtualisent l'ensemble de la machine, y compris les couches matérielles.
- **Conteneurs** ne virtualisent que les couches logicielles au-dessus du système d'exploitation, démarrent plus rapidement et consomment moins de mémoire.
![[container-vms 1.jpg]]
Les **conteneurs** incluent l'application et ses **dépendances** (dependencies), permettant une exécution autonome. Ils sont souvent utilisés avec des **microservices** (microservices) communiquant via des **API** ou des méthodes légères comme **REST** ou **gRPC**.

### Kubernetes

**Kubernetes** gère les **charges de travail** et **services conteneurisés**. Il permet l'**orchestration**, la **scalabilité**, les **déploiements** et les **rollback**.

- **Google Kubernetes Engine** (**GKE**) est un service **Kubernetes géré** dans le cloud, utilisant des **clusters** (clusters) d'**instances Compute Engine** (Compute Engine instances).
- GKE facilite le **déploiement**, l'**ajustement de capacité** et la **surveillance** des applications.

### GKE Autopilot

**GKE Autopilot** simplifie la gestion des clusters Kubernetes en facturant uniquement les **pods** utilisés. Google Cloud gère automatiquement l'infrastructure, y compris les **nœuds**, la **mise à l'échelle** (scaling) et les **mises à jour**. Cela réduit la charge opérationnelle et optimise les coûts. Un **pod** est l'unité de base de déploiement dans **Kubernetes**. Il regroupe un ou plusieurs **conteneurs** (containers) qui partagent le même réseau, le même stockage et les mêmes ressources. Les conteneurs au sein d’un **pod** sont exécutés sur le même hôte et communiquent entre eux facilement.

### Comparaison

| **Caractéristique**              | **GKE (Google Kubernetes Engine)**                | **GKE Autopilot**                       |
| -------------------------------- | ------------------------------------------------- | --------------------------------------- |
| **Gestion des nœuds**            | Manuelle (vous gérez les nœuds et les ressources) | Automatique (Google gère les nœuds)     |
| **Facturation**                  | Facturation basée sur les nœuds (VM)              | Facturation basée sur les pods utilisés |
| **Contrôle de l'infrastructure** | Élevé (vous configurez et gérez les nœuds)        | Limité (Google gère l'infrastructure)   |
| **Mise à l'échelle**             | Manuelle (vous gérez le scaling des nœuds)        | Automatique (scaling géré par Google)   |
| **Complexité opérationnelle**    | Plus élevé (besoin de gestion et maintenance)     | Réduit (simplification de la gestion)   |

### Cloud Run

**Cloud Run** est une plateforme **serverless** pour exécuter des applications conteneurisées sans gérer l'infrastructure. Elle ajuste automatiquement les ressources selon le trafic, idéal pour des applications **sans état** (stateless) et avec des besoins de **scaling** rapide.
#### Comparaison

|**Service**|**Description**|**Idéal pour**|
|---|---|---|
|**GKE**|**Kubernetes** géré pour les applications complexes.|Contrôle approfondi sur les clusters.|
|**Cloud Run**|**Serverless** pour les applications simples et légères.|Applications légères avec **scaling** rapide.|

### Conclusion

- **GKE** : Contrôle avancé pour des applications complexes.
- **Cloud Run** : Solution **serverless** pour des applications simples et scalables.