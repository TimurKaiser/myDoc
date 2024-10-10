# Representational State Transfer API

L'API REST permet de concevoir des services WEB qui utilisent les méthodes HTTP (HyperText Transfer Protocole) pour la communication entre le client et le serveur.
REST est basé sur des principes qui permettent de créer des services web 
stateless, c'est-à-dire que chaque requête du client contient toutes les informations nécessaires pour être traitée par le serveur, sans nécessiter de mémoire de la part du serveur entre les requêtes.


## Principe de base du REST

**Resources (Ressources)** :

Les ressources sont les objets ou les données que l'API gère, comme des utilisateurs, des produits ou des articles. Chaque ressource est identifiée par une URL (Uniform Resource Locator).
Par exemple dans l'api `https://api.example.com/users/123` pourrait représenter un utilisateur spécifique avec l'ID 123.


**Stateless (Sans État)** :

Chaque requête du client au serveur doit contenir toutes les informations nécessaires pour comprendre et traiter la requête. Un système **stateless** ne garde pas de mémoire entre les requêtes. Chaque requête est indépendante et contient toutes les informations nécessaires pour être traitée.
Les requêtes sont stateless du client eu serveur mais également du serveur au client
Chaque requête est donc complète et autonome et le serveur ne se souvient pas des interactions passées.


**Utilisation des Codes de Statut HTTP** :
Les API REST utilisent les codes de statut HTTP pour indiquer le résultat d'une requête. Par exemple :


- `200 OK` : Requête réussie.
- `201 Created` : Ressource créée avec succès.
- `204 No Content` : La requête a réussi mais il n'y a pas de contenu à renvoyer.
- `400 Bad Request` : La requête est invalide.
- `404 Not Found` : La ressource demandée n'existe pas.
- `500 Internal Server Error` : Erreur côté serveur.




**Représentations** :
Les ressources peuvent avoir différentes représentations, comme JSON, XML, ou HTML. JSON est le format de données le plus couramment utilisé dans les API REST modernes.





 **HATEOAS (Hypermedia As The Engine Of Application State)** :

C'est un principe qui suggère que les réponses de l'API REST devraient inclure des liens vers d'autres ressources, permettant aux clients de découvrir de manière dynamique les actions possibles sur les ressources.


# Les méthodes HTTP


Les méthodes HTTP ( Hyper Text Transfer Protocol ) sont des verbes utilisés par les 
clients, on les appels ainsi car ils indiquent une action à effectuer.  Les principaux méthodes sont :

- **GET** : "Lire" ou "obtenir" des informations. Par exemple, une demande GET pourrait récupérer les donner d'un utilisateur.
- **POST** : "Créer" une nouvelle ressource. Par exemple, une demande POST pourrait être utilisée pour créer un nouveau compte utilisateur ou pour mettre à jour les informations de profil d'un utilisateur.
- **PUT** : "Remplacer" ou "mettre à jour" une ressource. Par exemple, une demande PUT pourrait remplacer une ancienne image par une nouvelle.
- **DELETE** : "Supprimer" une ressource. Par exemple, une demande DELETE pourrait supprimer un compte utilisateur.


## Exemple en code en JS

```javascript
// GET request  
  
const request = new Request('https://example.com/');  
  
request.method = 'GET';  
  
const response = await fetch(request);  
  
// POST request  
  
const request = new Request('https://example.com/users', {  
  method: 'POST',  
  body: JSON.stringify({  
    name: 'John Doe',  
    email: 'johndoe@example.com',  
  }),  
});  
  
const response = await fetch(request);  
  
// PUT request  
  
const request = new Request('https://example.com/users/123', {  
  method: 'PUT',  
  body: JSON.stringify({  
    name: 'Jane Doe',  
    email: 'janedoe@example.com',  
  }),  
});  
  
const response = await fetch(request);  
  
// DELETE request  
  
const request = new Request('https://example.com/users/123', {  
  method: 'DELETE',  
});  
  
const response = await fetch(request);
```