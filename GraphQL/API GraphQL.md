 
# GraphQueryLanguage

GraphQL a été développé par Facebook pour répondre aux problématiques des API REST qui ne sont pas toujours adaptées aux besoins des réseaux sociaux. En effet, une API REST permet de communiquer un ou plusieurs éléments, mais GraphQL permet également de représenter les relations entre eux, le tout sous forme de graphe. Cela est particulièrement utile pour la lecture de données et leurs relations dans un réseau social.

Les données dans un réseau social, par exemple, peuvent être représentées par des nœuds et des liens, ces derniers formant le graphe. L'objectif de GraphQL est de faire des requêtes pour parcourir ce graphe, en accédant à des objets de différentes natures.


# Les différentes  requêtes :

Il existe trois types de requêtes dans GraphQL : **les queries**, **les mutations** et **les subscriptions**. Chacune a ses propres fonctionnalités.

- **Query** : Permet la lecture de données, comparable à la requête GET en REST.
- **Mutation** : Permet la modification de données, y compris la création, la mise à jour et la suppression. Elle combine les requêtes POST, PUT, PATCH et DELETE.
- **Subscription** : Permet de recevoir des mises à jour en temps réel, par exemple chaque fois qu'un nouvel utilisateur est ajouté.


# Avantage de GraphQL

L'API GraphQL offre plusieurs avantages :

- **Introspection** : Permet au client d’interroger l'API pour découvrir exactement toutes les actions possible à faire avec l'API, sans avoir besoin de consulter une documentation séparée.
- **Requêtes Composées** : En une seule query, on peut obtenir toutes les données nécessaires. Par exemple, pour obtenir les détails d'un utilisateur et la liste de ses articles, on peut faire une seule requête GraphQL.

En REST, il faut  potentiellement  à faire deux requêtes :

 - Une requête pour obtenir les informations de l'utilisateur (`/user/123`).
 -  Une autre requête pour obtenir la liste des articles de cet utilisateur (`/user/123/posts`).

Avec GraphQL,  on peut faire tout cela en une seule requête :

```graphql
{
  user(id: "123") {
    name
    email
    posts {
      title
      content
    }
  }
}
```

### Avantages :

- **Moins de surcharge réseau** : Une seule requête HTTP est envoyée, ce qui réduit le nombre de connexions et améliore la performance.
- **Simplicité** : Le client reçoit une réponse structurée en une seule fois, facilitant le traitement des données.
- **Optimisation** : On demande uniquement ce dont nous avons besoin, pas plus.

### Désavantages :

- **Surcharge potentielle** : Une requête complexe peut demander de nombreuses relations, ce qui peut surcharger l'API.
- **Problème de N+1** : Si les relations entre les données ne sont pas bien gérées, cela peut entraîner des problèmes de type "N+1", où une requête supplémentaire est faite pour chaque élément d'une liste, augmentant ainsi le nombre de requêtes exécutées en arrière-plan. Pour éviter cela, les développeurs doivent mettre en place des mécanismes de limitation de débit (throttling) pour contrôler la profondeur des requêtes.
- **Mise en place et maintenance** : La mise en place et la sécurisation des API GraphQL peuvent être plus complexes. Les attaques potentielles, telles que les attaques N+1 et la surcharge du serveur, doivent être prises en compte. L'introspection peut être exploitée pour surcharger le serveur ou pour identifier des champs sensibles, permettant ainsi d'extraire plus de données que prévu.

C'est l'une des raisons pour lesquelles les API REST sont encore plus courantes que les API GraphQL.


# Les graphiques avec GraphQl



En combinant la puissance de GraphQL pour relier différentes données et les capacités de SVG pour les représenter visuellement, on obtient un outil formidable pour analyser et comprendre des informations complexes, offrant une vue d'ensemble claire et exploitable.

**GraphQL** est conçu pour interroger plusieurs sources de données à la fois, ce qui est particulièrement utile lorsqu'on veut créer des graphiques complexes qui nécessitent des informations provenant de différents points d'origine. 

Ces données, une fois consolidées, peuvent être utilisées pour générer un  [[Graphique SVG]] non seulement affichent des informations, mais montrent aussi les relations entre elles. Par exemple, un graphique en radar ou un diagramme à bar pourrait illustrer les données Grâce aux  SVG, chaque élément peut être programmé pour réagir aux données, permettant une exploration interactive des relations complexes entre ces données.
