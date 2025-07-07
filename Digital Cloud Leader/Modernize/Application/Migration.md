Lorsqu'une entreprise modernise ses activités et les déploie dans le cloud, elle peut rencontrer des applications spécialisées qui ne sont pas compatibles avec les applications cloud natives. Dans ce cas, une migration de réhébergement, appelée également **Lift and Shift**, consiste à déplacer l'application d'un environnement sur site vers un environnement cloud, sans apporter de modifications à l'application elle-même.

### Avantages du réhébergement :

- **Réduction des coûts** : Les entreprises peuvent bénéficier des avantages financiers du cloud sans avoir à réécrire leurs applications.
- **Évolutivité** : La capacité à augmenter ou réduire les ressources en fonction de la demande.
- **Fiabilité** : Utilisation de l'infrastructure du cloud pour une meilleure disponibilité.
- **Sécurité accrue** : Les services cloud offrent une sécurité robuste et une gestion des risques.

### Inconvénients du réhébergement :

1. **Complexité** : Le processus de migration peut être complexe, nécessitant une planification minutieuse pour garantir la bonne gestion des ressources.
2. **Risque** : Toute migration vers le cloud comporte des risques potentiels. Il est donc essentiel d'évaluer les risques et de disposer d'un plan de secours en cas de problème.
3. **Dépendance vis-à-vis du fournisseur** : En optant pour le réhébergement, les entreprises peuvent devenir dépendantes d'un fournisseur cloud spécifique, ce qui peut compliquer une éventuelle migration vers un autre fournisseur à l'avenir.

### Solutions de Google Cloud pour migrer des applications anciennes :

- **Google Cloud VMware Engine** : Cette solution permet de migrer les charges de travail VMware existantes vers le cloud sans modifier l'architecture des applications ni réorganiser les opérations. Les entreprises peuvent continuer à utiliser leurs environnements VMware tout en tirant parti des avantages du cloud de Google, tels que l’évolutivité, la sécurité et la fiabilité. De plus, elles peuvent accéder à des services Google Cloud comme BigQuery, l'intelligence artificielle (IA), le machine learning (ML), et Google Kubernetes Engine pour moderniser leurs applications.

- **Google Cloud Bare Metal** : Cette solution offre des serveurs physiques dédiés dans le cloud, permettant aux organisations d'exécuter des charges de travail Oracle sur des serveurs **Bare Metal** (serveurs physiques sans virtualisation). Cela permet aux entreprises ayant des applications anciennes et critiques, comme celles utilisant des bases de données Oracle, de bénéficier des performances et de la flexibilité du cloud tout en maintenant des configurations personnalisées sur des serveurs physiques.

Un serveur **bare metal** est une infrastructure cloud qui vous offre une **machine physique entièrement dédiée** à votre organisation, sans virtualisation partagée. Contrairement aux serveurs virtuels, où les ressources (comme le CPU, la mémoire, et le stockage) sont partagées entre plusieurs utilisateurs, un serveur bare metal vous permet d'accéder à **toute la puissance** de la machine pour vos applications.

### Conclusion :

Le réhébergement est une solution rapide et efficace pour déplacer les anciennes applications vers le cloud, mais elle présente aussi des défis. L’utilisation des services de migration de Google Cloud, tels que VMware Engine et Bare Metal, permet aux entreprises de moderniser progressivement leurs applications tout en tirant parti des avantages du cloud sans devoir tout refactoriser immédiatement.