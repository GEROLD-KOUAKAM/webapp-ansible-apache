# webapp-ansible-apache: déploiement d'un conteneur apache à l'aide de ansible

- Création d'un cluster ( 02 serveurs : un serveur ansible debian 9 qui joue le role de node manager et un autre serveur centos 7 qui joue le role de client)
- Creation d'un fichier webapp qui va contenir tous les fichiers du projet
- Création d'un fichier inventaire prod.yml  contenant un group prod avec comme seul membre notre client
- Creation d'un dossier group_vars qui va contenir un fichier prod qui contiendra les informations de connexion à utiliser par ansible (login + mot de passe)
- Création d'un playbook nommé deploy.yml permettant de déployer apache à l'aide de docker sur le client ( l'image utilisée est httpd et le port à exposer à l'extérieur est 80
- Task d'installation du gestionnaire de paquet pip pour python et docker pour son utlisation sur la machine cliente.
- tache réaliser sur le serveur client en tant que sudo admin et non root.
- Verification de la syntaxe du playbook avec la commande ansible-lint
