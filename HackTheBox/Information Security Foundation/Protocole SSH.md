Le protocole SSH marche avec un système de paire de clefs ;  privé et public. A l'aide de ces deux clefs le serveur et l’hôte peuvent s'identifier. Un channel sécuriser est donc ouvert avec un système de chiffrement et de déchiffrement à l'aide des clefs. Voir schéma ci dessous [[Draw SSH]]. Dans notre schéma il y'a un client SSH et un Serveur SSH, soit deux entité, mais il existe d'autre version avec 3 entité dans lequel notre serveur et notre hôte et séparer par un autre serveur SSH.

On peut rajouter d'autre sécurité, des pare-feu pour contrôler les ports, filtrer les IP, surveiller le trafic tout cela pour administré le système. Des outils de protection existe, comme Fail2Ban.

Il est important de sécuriser aussi au niveau des clients, en configurant par exemple l'A2F ou 2FA en anglais (2 Factor Authentification). Nous pouvons utiliser Google Authentificator par exemple qui vas générer pour chaque client une clé unique OTP (One-Time-Passxord) de 30s.
