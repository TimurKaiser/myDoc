### Gestion des Identités et des Accès dans GCP : Les 3A

Les trois aspects essentiels de la gestion des identités et des accès dans le cloud sont l'**authentification (authentication)**, l'**autorisation (authorization)** et l'**audit (audit)**. Ces processus permettent de sécuriser l'accès aux ressources, de gérer les droits des utilisateurs, et de surveiller l'utilisation des ressources cloud.

#### 1. **Authentification (Authentication)**

L'authentification est le processus de vérification de l'identité d'un utilisateur ou d'un système avant qu'ils ne puissent accéder à une ressource. Elle repose sur des identifiants uniques tels que des **mots de passe (passwords)**, des **jetons physiques (security tokens)** ou des **données biométriques (biometrics)** (par exemple, empreintes digitales ou reconnaissance vocale).

La **validation en deux étapes (Two-factor Authentication - 2FA)**, ou **authentification multifacteur (Multi-factor Authentication - MFA)**, renforce la sécurité en demandant deux informations distinctes pour l'accès : par exemple, un mot de passe et un code reçu sur un téléphone via SMS, appel vocal, ou une application comme **Google Authenticator**.

#### 2. **Autorisation (Authorization)**

Une fois l'identité authentifiée, l'autorisation détermine les actions qu'un utilisateur ou un système peut effectuer sur le cloud. Elle repose sur un système de **contrôle des accès (access control)** où des **rôles (roles)** sont attribués aux utilisateurs en fonction de leur fonction et de leur position dans l'organisation.

Exemples de rôles :

- Un **administrateur système (system administrator)** peut gérer des comptes utilisateurs.
- Un utilisateur avec des **droits d'accès standard (standard access rights)** peut seulement consulter les informations disponibles.

Cela garantit que les utilisateurs disposent des permissions nécessaires sans dépasser leur niveau d'autorisation.

#### 3. **Audit (Audit)**

L'audit, également appelé traçabilité, joue un rôle essentiel dans la surveillance des actions réalisées sur un système. En recueillant et en analysant les **journaux d'activité (logs)**, l'audit permet de détecter les anomalies, les violations de sécurité et de vérifier la conformité des actions. Il fournit un historique détaillé des actions effectuées sur les ressources cloud, utile pour :

- Enquêter sur des incidents de sécurité.
- Suivre la **conformité (compliance)**.
- Évaluer la **performance système (system performance)**.

### Gestion des Identités et des Accès dans Google Cloud : IAM

Pour gérer les accès aux ressources dans Google Cloud, **Identity and Access Management (IAM)** est utilisé. IAM permet de :

- Créer et gérer des comptes utilisateur.
- Attribuer des rôles.
- Accorder ou révoquer des autorisations d'accès sur les ressources.
- Contrôler les activités des utilisateurs.
- Surveiller les stratégies de sécurité. 

IAM offre une approche centralisée et efficace pour la gestion des accès dans Google Cloud, contribuant à la protection des ressources numériques de l'entreprise. En intégrant IAM à la stratégie de sécurité de l'entreprise, il est possible de :

- Assurer un contrôle précis des accès.
- Améliorer la **visibilité (visibility)**.
- Gérer les ressources de manière centralisée.

Ainsi, IAM aide à protéger les données sensibles et à sécuriser l'infrastructure du cloud.

| **Aspects**                                  | **Description**                                                                                                                                                   |
| -------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Authentification**                         | Vérification de l'identité des utilisateurs ou systèmes pour accéder aux ressources. Cela peut être réalisé via des mots de passe, jetons physiques ou biométrie. |
| **Validation en deux étapes (2FA/MFA)**      | Sécurisation supplémentaire en demandant deux informations distinctes pour l'accès (ex : mot de passe + code envoyé).                                             |
| **Autorisation**                             | Détermination des actions qu'un utilisateur peut effectuer après son identification. Basé sur des rôles attribués.                                                |
| **Contrôle des accès**                       | Mécanisme pour attribuer des droits en fonction des rôles dans l'organisation.                                                                                    |
| **Audit**                                    | Surveillance des actions des utilisateurs et collecte des logs pour détecter les anomalies, les violations de sécurité, et garantir la conformité.                |
| **IAM (Gestion des identités et des accès)** | Gestion centralisée des utilisateurs, rôles et permissions pour sécuriser les ressources dans Google Cloud.                                                       |
