# 🐧 Commandes Linux Importantes

Ce fichier répertorie des commandes essentielles que vous pouvez utiliser sous Linux, que ce soit dans le **terminal** (bash ou shell). Ces commandes sont utiles pour gérer votre système, diagnostiquer des problèmes ou automatiser des tâches.

---

## 🤖 Commandes Utiles

| Commande                                              | Description                                                     | Exemple d'utilisation                                         | Nécessite des privilèges admin ? |
|--------------------------------------------------------|-----------------------------------------------------------------|---------------------------------------------------------------|----------------------------------|
| `echo [texte]`                                         | Affiche un texte dans le terminal.                             | `echo Bonjour, bienvenue dans le guide !`                     | false                            |
| `exit`                                                 | Ferme le terminal ou termine un script.                        | `exit`                                                         | false                            |
| `cd [répertoire]`                                      | Change le répertoire de travail actuel.                        | `cd /home/Utilisateur/Documents`                              | false                            |
| `mkdir [dossier]`                                      | Crée un nouveau dossier.                                       | `mkdir NouveauDossier`                                         | false                            |
| `rm [fichier]`                                         | Supprime un fichier.                                           | `rm fichier.txt`                                               | false                            |
| `rm -r [dossier]`                                      | Supprime un dossier et son contenu.                            | `rm -r DossierADelete`                                         | false                            |
| `cp [source] [destination]`                            | Copie un fichier ou un dossier vers un autre emplacement.      | `cp fichier.txt /chemin/vers/dossier/`                         | false                            |
| `mv [source] [destination]`                            | Déplace ou renomme un fichier ou un dossier.                   | `mv fichier.txt /nouveau/chemin/`                              | false                            |
| `cat [fichier]`                                        | Affiche le contenu d'un fichier dans le terminal.              | `cat fichier.txt`                                              | false                            |
| `nano [fichier]`                                       | Ouvre un fichier dans l'éditeur de texte Nano.                 | `nano fichier.txt`                                             | false                            |
| `touch [fichier]`                                      | Crée un fichier vide ou met à jour la date de modification.    | `touch nouveauFichier.txt`                                     | false                            |
| `ls`                                                   | Liste les fichiers et dossiers du répertoire actuel.           | `ls /home/Utilisateur`                                         | false                            |
| `ls -l`                                                | Affiche une liste détaillée des fichiers et dossiers.          | `ls -l /home/Utilisateur`                                      | false                            |
| `pwd`                                                  | Affiche le chemin complet du répertoire de travail actuel.     | `pwd`                                                          | false                            |
| `chmod [mode] [fichier]`                               | Modifie les permissions d'un fichier ou d'un dossier.          | `chmod 755 fichier.sh`                                         | true                             |
| `chown [utilisateur]:[groupe] [fichier]`                | Change le propriétaire ou le groupe d'un fichier ou d'un dossier. | `chown user:group fichier.txt`                                | true                             |
| `sudo [commande]`                                      | Exécute une commande avec les privilèges administrateur.       | `sudo apt update`                                              | true                             |
| `apt-get install [paquet]`                             | Installe un paquet sur les systèmes basés sur Debian (comme Ubuntu). | `sudo apt-get install firefox`                              | true                             |
| `yum install [paquet]`                                 | Installe un paquet sur les systèmes basés sur Red Hat (comme CentOS). | `sudo yum install vim`                                        | true                             |
| `df -h`                                                | Affiche l'espace disque utilisé et disponible.                 | `df -h`                                                        | false                            |
| `free -h`                                              | Affiche la mémoire RAM et l'espace d'échange utilisé et disponible. | `free -h`                                                    | false                            |
| `top`                                                  | Affiche les processus en cours et leur utilisation des ressources système. | `top`                                                        | false                            |
| `ps aux`                                               | Affiche une liste des processus en cours d'exécution.          | `ps aux`                                                       | false                            |
| `kill [PID]`                                           | Termine un processus par son identifiant (PID).                | `kill 1234`                                                    | true                             |
| `grep [motif] [fichier]`                               | Recherche un motif dans un fichier ou une sortie de commande. | `grep "Erreur" fichier.log`                                    | false                            |

---

## Explication des Commandes

- **`echo`** : Affiche du texte dans le terminal. Très utile pour afficher des messages ou tester des variables.
- **`exit`** : Ferme le terminal ou termine un script.
- **`cd`** : Change le répertoire de travail dans le terminal. Utilisé pour naviguer dans le système de fichiers.
- **`mkdir`** : Crée un nouveau dossier.
- **`rm`** : Supprime un fichier. Ajoutez `-r` pour supprimer un dossier et son contenu.
- **`cp`** : Copie des fichiers ou des dossiers d'un emplacement à un autre.
- **`mv`** : Déplace ou renomme un fichier ou un dossier.
- **`cat`** : Affiche le contenu d'un fichier texte dans le terminal.
- **`nano`** : Ouvre un fichier dans l'éditeur de texte Nano, utile pour modifier des fichiers texte rapidement.
- **`touch`** : Crée un fichier vide ou met à jour la date de modification d'un fichier existant.
- **`ls`** : Liste les fichiers et dossiers dans le répertoire courant. Utilisez `ls -l` pour plus de détails.
- **`pwd`** : Affiche le répertoire courant dans lequel vous vous trouvez.
- **`chmod`** : Modifie les permissions d'un fichier ou d'un dossier.
- **`chown`** : Change le propriétaire ou le groupe d'un fichier ou d'un dossier.
- **`sudo`** : Exécute une commande avec des privilèges administratifs.
- **`apt-get`** : Utilisé pour installer, mettre à jour et gérer les paquets sur les systèmes basés sur Debian/Ubuntu.
- **`yum`** : Utilisé pour installer, mettre à jour et gérer les paquets sur les systèmes basés sur Red Hat/CentOS.
- **`df`** : Affiche l'espace disque utilisé et disponible sur les systèmes de fichiers.
- **`free`** : Affiche la quantité de mémoire utilisée et libre sur le système.
- **`top`** : Affiche en temps réel les processus qui consomment le plus de ressources.
- **`ps`** : Affiche les processus en cours d'exécution.
- **`kill`** : Permet d'arrêter un processus en utilisant son identifiant (PID).
- **`grep`** : Utilisé pour rechercher un texte spécifique dans un fichier ou dans la sortie d'une commande.

---

Ce tableau des commandes Linux vous aide à gérer votre système et à effectuer diverses opérations quotidiennes. Si vous avez des questions supplémentaires ou avez besoin de plus de détails, n'hésitez pas à demander !
