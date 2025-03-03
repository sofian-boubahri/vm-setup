# 🖥️ Commandes Windows Importantes

Ce fichier répertorie des commandes essentielles que vous pouvez utiliser sous Windows, que ce soit dans **l'invite de commandes (CMD)** ou **PowerShell**. Ces commandes sont utiles pour gérer votre système, diagnostiquer des problèmes ou automatiser des tâches.

---

## 🤖 Commandes Utiles

| Commande                                                | Description                                                     | Exemple d'utilisation                                     | Nécessite des privilèges admin ?  |
|----------------------------------------------------------|-----------------------------------------------------------------|-----------------------------------------------------------|-----------------------------------|
| `echo [texte]`                                           | Affiche un texte dans la fenêtre de commande.                  | `echo Bonjour, bienvenue dans le guide !`                | false                             |
| `exit`                                                   | Ferme l'invite de commande ou PowerShell.                      | `exit`                                                    | false                             |
| `cd [répertoire]`                                        | Change le répertoire de travail actuel.                        | `cd C:\Users\NomUtilisateur\Documents`                    | false                             |
| `mkdir [dossier]`                                        | Crée un nouveau dossier.                                       | `mkdir NouveauDossier`                                   | false                             |
| `del [fichier]`                                          | Supprime un fichier.                                           | `del fichier.txt`                                         | false                             |
| `net user [utilisateur] [mot_de_passe] /add`             | Crée un nouvel utilisateur.                                    | `net user nouvelUtilisateur motDePasse123 /add`          | true                              |
| `cat [fichier]`                                          | Affiche le contenu d'un fichier dans PowerShell ou WSL.        | `cat C:\chemin\vers\monfichier.txt`                       | false                             |
| `move [source] [destination]`                             | Déplace un fichier ou un dossier vers un autre emplacement.    | `move fichier.txt C:\nouveau\emplacement\`                | false                             |
| `rename [ancien_nom] [nouveau_nom]`                       | Renomme un fichier ou un dossier.                              | `rename fichier.txt fichier_renomme.txt`                  | false                             |
| `notepad [fichier]`                                      | Ouvre un fichier dans l'éditeur de texte Notepad.              | `notepad C:\chemin\vers\monfichier.txt`                   | false                             |


