# Application Programming Interface


## API WEB

Une API est une interface, c'est-à-dire le lien entre deux entités. L'API établit une connexion entre deux programmes (par exemple, une base de données, une bibliothèque logicielle, etc.). Il existe plusieurs types d'API, la plus connue étant l'API Web, qui elle-même se décline en plusieurs formats, comme l'[[API REST]] et l'[[API GraphQL]].

L'API est au cœur même du Web 2.0, permettant de contourner les limitations liées à l'interface utilisateur (UI). Dans le Web 1.0, il était nécessaire de rafraîchir la page pour accéder à de nouvelles données : l'utilisateur cliquait quelque part, et le serveur renvoyait un fichier HTML et CSS que le navigateur devait recharger.

Avec le Web 2.0, qui utilise principalement des bibliothèques comme React, Vue, ou Angular, l'API est chargée en même temps que le code de la page par le navigateur. L'API permet une mise à jour dynamique de la page sans avoir besoin de la recharger entièrement. Par exemple, lorsqu'on like une vidéo, la page ne se recharge pas et la vidéo ne s’arrête pas, mais le compteur de likes est tout de même mis à jour.

Il existe plusieurs méthodes pour interagir avec une API et le serveur : les méthodes GET, POST, etc. Le serveur, quant à lui, renvoie des données dans un format spécifique, généralement en JSON (JavaScript Object Notation), qui a succédé à XML. JSON est plus lisible pour les humains et plus léger.

À noter qu'il est possible de faire tout cela de manière asynchrone grâce à AJAX (Asynchronous JavaScript and XML). Malgré son nom, AJAX est souvent utilisé pour envoyer et recevoir des données au format JSON, car ce dernier est plus performant et compatible avec JavaScript.