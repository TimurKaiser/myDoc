## **Souveraineté et Résidence des Données dans Google Cloud**

| **Concept**                                       | **Définition**                                                                                | **Exemple & Application**                                                                                                            |
| ------------------------------------------------- | --------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **Souveraineté des données** (_Data Sovereignty_) | Principe juridique selon lequel les données sont soumises aux lois du pays où elles résident. | Le RGPD impose aux entreprises de respecter les lois européennes sur la protection des données, même si elles sont stockées hors UE. |
| **Résidence des données** (_Data Residency_)      | Localisation physique du stockage et du traitement des données.                               | Certains pays exigent que les données personnelles de leurs citoyens soient stockées sur leur territoire.                            |

## **Gestion de la Résidence des Données dans Google Cloud**

| **Solution Google Cloud**                  | **Description**                                                                                                             |
| ------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------- |
| **Choix des régions**                      | Google Cloud permet de choisir l'emplacement de stockage des données à travers différentes régions et centres de données.   |
| **Conformité aux réglementations locales** | Google Cloud garantit que les données restent stockées dans la région sélectionnée, conformément aux conditions de service. |
| **IAM et règles d’administration**         | Mise en place de contraintes pour empêcher le stockage des données dans une région non autorisée.                           |
| **VPC Service Controls**                   | Restriction des accès aux données via des périmètres réseau sécurisés.                                                      |
| **Filtrage des adresses IP**               | Limitation des accès utilisateurs en fonction de leur adresse IP.                                                           |
| **Google Cloud Armor**                     | Protection supplémentaire en restreignant les emplacements de trafic autorisés pour les équilibreurs de charge externes.    |

### **Bénéfices pour les Entreprises**

- Respect des exigences légales en matière de résidence et souveraineté des données.
- Conformité renforcée avec les réglementations internationales et locales.
- Contrôle et sécurisation avancés des données stratégiques dans Google Cloud.
