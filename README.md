# Environnement Unix

Pour travailler sur le cours UNIX, vous aurez besoin d'un environnement UNIX utilisable. Ce que j'appelle un environnement UNIX c'est un terminal avec un shell qui s'exécute (e.g. `bash`), les utilitaires par defaut (`ls, grep, sed` etc.), les pages `man` correctement installées, un compilateur C (comme `gcc`), et un éditeur de texte comme `emacs`, `vim` ou eventuellement `nano`.

Sur cette page, vous trouverez quelques pistes pour installer un envrionnement UNIX depuis Windows et OSX. Attention: je ne suis pas un utilisateur expert, ni de Windows, ni de OSX donc il est possible que ces informations soient érronées ou insuffisantes. En cas de difficultés, je vous conseille avant tout de discuter avec vos camarades qui utilisent le même système que vous. Si vous avez des commentaires utiles à ajouter à cette page, n'hésitez pas à m'envoyer un mail (voir à la fin de ce documents).

Depuis Windows
==============

Avec une machine virtuelle
---

Une machine virtuelle est un programme capable de simuler le fonctionnement d'un ordinateur (machine) virtuel(le).
Si votre ordinateur est un PC sous Windows, vous pouvez installer une machine virtuelle comme Virtual Box et y installer le système Ubuntu.  Vous pouvez ainsi installer n'importe quel système d'exploitation dans la machine virtuelle, sans modifier toucher au système de base de la machine physique, et donc, sans risquer de tout casser. 

Vous pouvez trouver de nombreux tutoriels pour installer une machine virtuelle avec Ubuntu sur internet, par exemple, celui ci me semble pas mal: [https://www.papergeek.fr/comment-installer-une-machine-virtuelle-linux-dans-windows-10-81428"](https://www.papergeek.fr/comment-installer-une-machine-virtuelle-linux-dans-windows-10-81428)

Sans machine virtuelle
---

Vous pouvez également installer un environnement Unix sans utiliser de machine virutelle, c'est probablement la solution la plus simple. Vous n'êtes pas complétement immergés dans un environement Unix, mais cela vous permet tout de même de pratiquer l'utilisation des commandes shell. 

Il y a au moins deux manières de faire ça:

### Cygwin 

Crée par la communauté des utilisateurs de Unix pour le système Windows. 

https://www.cygwin.com/

### Le sous système windows pour Linux

Crée par Microsoft. 

Voici [la doc](https://docs.microsoft.com/fr-fr/windows/wsl/about) et [un tutoriel](https://www.youtube.com/watch?v=Cvrqmq9A3tA) qui décrit toute l'installation étape par étape.


Depuis OSX
==========

Si votre ordinateur est un Mac, vous pouvez également installer une machine virtuelle (voir section précédente). Ceci étant, le système OSX étant un système compatible Unix, vous pouvez aussi vous passer d'une machine virtuelle, et faire les exercices directement sur votre système OSX. Ça demande un peu de bricolage et il peut y avoir quelques différences avec le système Ubuntu que nous avons utilisé pour concevoir les TPs, mais c'est une bonne solution quand même, et c'est un outil très utilisé par les utilisateurs Mac qui veulent profiter des avantages d'un environnement unix donc je vous encourage à faire ça. 

Pour disposer des outils dont vous allez avoir besoin pour faire les TP, il faut que vous trouviez le terminal dans OSX, et que vous installiez Homebrew. Homebrew, est un gestionnaire de paquet, qui vous permettra d'installer des paquets, c'est à dire des archives qui contiennent des programmes. Pour installer Homebrew, ouvrez un terminal dans OSX et tapez la commande suivante:

  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

Une fois que homebrew est installé, vous pouvez installer des paquets avec la commande

  brew install <nom_du_paquet>

par exemple, brew install emacs ou brew install gcc pour installer emacs ou gcc. Plus d'info sur le site de homebrew [ici](https://brew.sh/index_fr).\

**Note:** les utilisateurs de Mac me signalent que c'est parfois plus simple d'utiliser le gestionnaire de paquet de xcode en tappant la commande suivante:

  xcode-select ---install

Installer Linux/Ubuntu sur votre machine en Dual Boot
=====================================================

Si vous êtes motivé(e), vous pouvez également installer Ubuntu, directement sur votre machine en plus de votre système de base (on parle de *dual boot*), mais attention, une mauvaise installation pour vous empêcher de démarrer sur l'un ou l'autre système. Voici le tutoriel officiel pour installer Ubuntu : <https://ubuntu.com/tutorials/tutorial-install-ubuntu-desktop>.

Linux LIVE-USB
======

Idée : Linux est installé sur une clef USB bootable. 

Voir ce [lien](https://doc.ubuntu-fr.org/live_usb) 

Mettre à jour ce document
=========================

Si vous trouvez des erreurs, si vous voulez proposer des précisions ou de nouvelles manières d'installer un environnement Unix, n'hésitez pas à m'envoyer vos suggestions sur mon adresse mail (prenom.nom @ dauphine.psl.eu), ou mieux des *pull requests*.

Benjamin Negrevergne
