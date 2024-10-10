# Les Hyperviseurs
- **VMWare**
- **VirtualBox**


Les Hyperviseurs permettent de crée des OS (Opérating Système) comme [[Windows]], MacOS, [[ParrotOS]] etc... , par dessus notre OS principale ; des Machines Virtuels (VM).
Il existe un format standard  pour emballer des VM pour en faire des fichier. C'est le format OVF (Open Virtualisation Format), il vas nous permettre d'importer et exporter des VM. Il nous facilite donc le partage et la migration de VM.

Les Hyperviseur permettent également de virtualiser des serveurs, on appel ça des [[Draw VPS]] (Virtual Private Server). A partir d'un serveur physique nous pouvons crée des VPS des serveurs dissocié des uns et des autres auquel  on peut alloué des ressources du serveur physique (CPU, RAM, Stockage). Souvent des serveurs physique sont loué à des hébergeurs.

Il est important de bien configurer  son VPS le choix des différent protocole est important, comme l'IPv6 qui permet un large choix d'adresse IP et une meilleure gestion des pare-feu.
De plus il permet d'éviter le spoofing.
Il faut également  sécuriser les communications entre le client et le serveur, pour empêcher une attaque (MitM) Man-in-the-Midal. Pour eviter cela nous utiliserons le protocole [[Protocole SSH]] (Secure Shell Protocol).
## Format

Il y'a plusieurs format et modèles de fichier pour nos VM. Les fichier OVF (Open Virtualization Format) et OVA (Open Virtualization Appliance). Le format OVA est intéressant pour pouvoir  déployer notre VM. Le OVF quand a lui est utile pour pouvoir migrer notre machine.


# Les conteneuriseurs
- **Docker**

Les conteneuriseurs comme [[Docker]] permettent de crée des "conteneurs", une solution de virtualisation qui est plus légère.  Au leu d’intégrer un OS celui-ci partage la puissance du noyau hôte. Il contient à l'intérieur toutes les dépendances besoins pour une applications.   

Schéma de différence entre un conteneur et une VM [[Draw VM VS Docker]].

### Comparaison visuelle

|                                | Machines Virtuelles                       | Conteneurs                                                                                                          |
| ------------------------------ | ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Isolation**                  | Fort, OS complet pour chaque VM           | Modéré, partage du noyau de l'OS de l'hôte                                                                          |
| **Poids**                      | Lourd (OS complet, plus de ressources)    | Léger (partage du noyau, moins de ressources)                                                                       |
| **Démarrage**                  | Plus lent                                 | Très rapide                                                                                                         |
| **Utilisation des ressources** | Plus élevé                                | Plus efficace                                                                                                       |
| **Portabilité**                | Bonne, mais dépend de l'hyperviseur       | Très bonne, conteneurs peuvent être exécutés n'importe où où Docker (ou un autre runtime de conteneur) est installé |
| **Cas d'utilisation**          | Environnements de test, serveurs virtuels | Déploiement d'applications, microservices                                                                           |


# Les différents types d'Hyperviseur

## Hyperviseur de Type 1 (Bare-Metal) 

Les hyperviseurs de type 1, également connus sous le nom d'hyperviseurs "bare-metal", fonctionnent directement sur le matériel de l'hôte, sans passer par un système d'exploitation intermédiaire. Voici leurs principaux avantages et utilisations :

1. **Performance Optimale** : Étant donné qu'ils accèdent directement aux ressources matérielles, les hyperviseurs de type 1 offrent des performances supérieures par rapport aux hyperviseurs de type 2. Ils sont capables de gérer efficacement les ressources comme le CPU, la mémoire et le stockage, ce qui se traduit par une meilleure performance des machines virtuelles.

2. **Isolation et Sécurité** : Les hyperviseurs de type 1 offrent une isolation stricte entre les différentes machines virtuelles. Cela signifie qu'un problème dans une VM n'affectera pas les autres VMs ni l'hyperviseur lui-même. Cette isolation renforce la sécurité et la stabilité des environnements virtualisés.

Il existe aussi des KVM (Kernel-based Virtual Machine) Hyperviseur de Type 1 malgré le fait qu'il utilise un OS en base. C'est une technologie qui transforme le Noyau Linux en Hyperviseur.

## Hyperviseur de Type 2 (Hosted)

Il fonctionne au-dessus d'un système d'exploitation hôte et s'appuie sur l'OS pour gérer les appels matériels. C'est le cas de la plus part des VM et des Hyperviseurs : VMware Workstation, VirtualBox.
