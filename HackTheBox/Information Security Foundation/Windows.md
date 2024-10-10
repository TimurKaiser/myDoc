Windows est l'OS le plus utilisé, nous devons avoir une VM Windows. Il n'est initialement pas construit pour notre activité mais on peut l'améliorer. Il existe de plus en plus de fonctionnalité qui nous améliore la tache, comme WSL (Windows Subsytem for Linux). 
Cette fonctionnalité permet d’exécuter des applications et des commandes Linux sur un terminal.

Néanmoins il faut exclure certaines fonctionnalité de Windows pour pouvoir permettre à nos script, nos outils de fonctionner correctement. Les politiques de scannages de Windows peuvent mettre en quarantaine nos outils.  Sand oublier le fait que WIndows n'a pas été crée pour ce genre d'utilisation donc nous devons installer des outils d'optimisations.


# PSWindowsUpdate

Nous effectueront nos mise à jour manuellement avec l'outil PSWindowsUpdate (module PowerShell pour gérer les mises à jours etc... ) sur le terminal PowerShell. Le  PowerShell est
un langage qui permet d’interagir avec le système d'exploitation.


# Chocolatey

Nous utiliserons Chocolatey un gestionnaire de packet, tout comme APT (Advanced Package Tool) il ne permet d'installer des applications, des tools etc.. avec l'invite de commande.
 ```powershell-session
//telecharger
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

// choco pour appeler
// documentation https://docs.chocolatey.org/en-us/choco/commands/install/

// upgrade
choco upgrade chocolatey -y 

// les différentes commandes :
choco info vscode
choco install python vscode git wsl2 openssh openvpn 

// appliquer les mises à jours
RefreshEnv
```



# Windows Subsytem for Linux

Il existe une fonctionnalité  très intéressante le [[Draw WSL2]]. Il permet aux systèmes d'exploitation Linux de fonctionner en même temps que notre installation Windows. Cela peut nous aider en nous donnant un espace pour exécuter des outils développés pour Linux directement à l'intérieur de notre hôte Windows sans avoir besoin d'un programme hyperviseur ou d'une installation d'une application tierce telle que VirtualBox ou Docker. 

