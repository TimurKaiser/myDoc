# Contrôle des Accès aux Ressources 


Le cloud computing requiert une gestion rigoureuse des accès aux ressources. Contrairement aux infrastructures sur site qui utilisent des contrôles d'accès physiques, Google Cloud fournit un modèle de gestion des accès basé sur une hiérarchie des ressources.

## Hiérarchie des Ressources Google Cloud

La hiérarchie des ressources est une structure arborescente qui organise les ressources en groupes logiques, facilitant ainsi la gestion et le contrôle des accès.

![[Hierarchy.png]]
### Niveaux de la hiérarchie

| Niveau                                      | Description                                                                                |
| ------------------------------------------- | ------------------------------------------------------------------------------------------ |
| **Nœud d'organisation (Organization Node)** | Regroupe tous les projets et dossiers d'une entreprise.                                    |
| **Dossiers (Folders)**                      | Organisation de projets et d'autres dossiers pour affiner la gestion des accès.            |
| **Projets**                                 | Conteneurs de ressources, servant de point central pour les permissions et la facturation. |
| **Ressources**                              | Machines virtuelles (VM), buckets Cloud Storage, tables BigQuery, etc.                     |


## Gestion des Accès via les Stratégies

Une **stratégie (policy)** est un ensemble de règles d’accès définissant qui peut utiliser une ressource et comment elle peut être exploitée.

### Principes clés

1. **Attribution granulaire** : les autorisations peuvent être définies au niveau des ressources, des projets ou des dossiers.
2. **Héritage et propagation** : les permissions appliquées à un niveau supérieur sont automatiquement transmises aux niveaux inférieurs.
3. **Principe du moindre privilège** : les utilisateurs ne reçoivent que les droits strictement nécessaires, renforçant ainsi la sécurité.
4. **Audit et supervision** : suivi et analyse des modifications des autorisations pour une meilleure conformité et responsabilisation.

## Avantages de la Hiérarchie des Ressources

- **Gestion centralisée et simplifiée** des accès.
- **Propagation automatique des autorisations**, réduisant la complexité de configuration.
- **Amélioration de la sécurité et de la conformité** grâce à un contrôle rigoureux des accès.
- **Visibilité accrue et meilleure auditabilité** des activités.

## Conclusion

Comprendre et exploiter la hiérarchie des ressources dans Google Cloud permet d'assurer une gestion efficace des accès et de renforcer la sécurité des environnements cloud.