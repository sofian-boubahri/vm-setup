# Dual Boot sur VMware : Windows et Linux

Ce guide vous explique comment configurer un **dual boot** entre **Windows** et **Linux** sur VMware Workstation. Vous pourrez ainsi avoir les deux systèmes d'exploitation sur la même machine virtuelle et choisir lequel démarrer lors du lancement de la VM.

## Prérequis

Avant de commencer, assurez-vous de disposer des éléments suivants :

1. **VMware Workstation Pro** ou **VMware Workstation Player** installé sur votre machine hôte.
   - Vous pouvez télécharger VMware ici : https://www.vmware.com/products/workstation-pro.html
2. Un fichier **ISO** de **Windows** (si vous ne l'avez pas encore, vous pouvez le télécharger depuis : https://www.microsoft.com/en-us/software-download/windows10)
3. Un fichier **ISO** de **Linux** (Ubuntu, Debian, ou autre distribution. Vous pouvez télécharger Ubuntu ici : https://ubuntu.com/download/desktop)
4. Un **espace disque suffisant** pour les deux systèmes d'exploitation.

## Étapes pour ajouter un dual boot entre Windows et Linux

### 1. Créer une machine virtuelle pour Windows (si ce n'est pas déjà fait)

Si vous avez déjà une machine virtuelle Windows, vous pouvez sauter cette étape. Sinon, suivez ces étapes pour créer une machine virtuelle pour Windows :

1. Ouvrez **VMware Workstation**.
2. Cliquez sur **Créer une nouvelle machine virtuelle**.
3. Choisissez **Installer un système d'exploitation ultérieurement**.
4. Sélectionnez **Microsoft Windows** comme système d'exploitation et la version correspondant à votre ISO de Windows.
5. Donnez un nom à votre machine virtuelle (par exemple **Windows-VM**).
6. Configurez la taille de votre disque virtuel (recommandé : au moins 60 Go pour Windows).
7. Attachez le fichier **ISO** de Windows et démarrez la machine virtuelle pour effectuer l'installation de Windows.

### 2. Ajouter un disque dur supplémentaire pour Linux

Une fois Windows installé sur votre machine virtuelle, vous devez ajouter un disque dur virtuel supplémentaire pour installer Linux.

1. **Éteignez** la machine virtuelle Windows si elle est en cours d'exécution.
2. Sélectionnez la machine virtuelle Windows dans VMware Workstation et cliquez sur **Paramètres**.
3. Dans la fenêtre des paramètres de la machine virtuelle, cliquez sur **Ajouter** en bas à gauche pour ajouter un nouveau périphérique.
4. Sélectionnez **Disque dur** et cliquez sur **Suivant**.
5. Choisissez **Créer un nouveau disque virtuel**.
6. Configurez la taille du disque pour Linux (recommandé : au moins 40 Go) et choisissez un format de disque virtuel.
7. Cliquez sur **Terminer** pour ajouter le disque dur.

### 3. Ajouter un CD-ROM avec l'ISO de Linux

Vous devez maintenant ajouter un CD-ROM virtuel avec l'ISO de la distribution Linux que vous souhaitez installer.

1. Dans les paramètres de la machine virtuelle, sélectionnez **CD/DVD (IDE)**.
2. Cochez l'option **Utiliser un fichier ISO** et sélectionnez le fichier ISO de Linux que vous avez téléchargé.
3. Assurez-vous que l'ordre de démarrage est correctement configuré dans la machine virtuelle pour démarrer d'abord depuis le **CD/DVD** (ISO) avant le disque dur.

### 4. Configurer le dual boot avec GRUB

Une fois les deux systèmes installés, vous devrez configurer un **chargeur de démarrage** (GRUB) pour pouvoir choisir entre **Windows** et **Linux** au démarrage.

1. Lancez votre machine virtuelle avec le système Linux.
2. Lors de l'installation de Linux, assurez-vous que l'installateur détecte le disque dur Windows comme un autre système d'exploitation et installe **GRUB** (le chargeur de démarrage).
3. Si l'installation de GRUB ne se fait pas correctement, vous pouvez installer GRUB manuellement en démarrant sur un **live CD** de Linux et en exécutant des commandes pour installer et configurer GRUB.

### 5. Finaliser la configuration du dual boot

1. Une fois l'installation de Linux terminée, redémarrez la machine virtuelle.
2. Vous devriez voir un menu GRUB au démarrage, vous permettant de choisir quel système d'exploitation démarrer (Windows ou Linux).
3. Si GRUB ne s'affiche pas ou si Windows démarre directement, vous devrez peut-être réinstaller **GRUB** à l'aide d'un Live CD ou ajuster les paramètres de démarrage dans VMware.

## Conclusion

Vous avez maintenant un **dual boot** entre **Windows** et **Linux** sur VMware. Chaque fois que vous redémarrerez votre machine virtuelle, vous pourrez choisir le système d'exploitation à démarrer via le menu GRUB.
