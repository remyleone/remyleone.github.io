---
layout: article
teaser: Some useful UNIX commands
description: Useful UNIX commands
---

TODO: Move this cheat sheet to english but google (translate) can help
you meanwhile ;) 

General commands
-----------------

|Command |Meaning |
|:-----: |------- |
| !! | Commande précédente|
| 7 signal | Liste des signaux|
| arch | Affiche l'architecture de la machine|
| arp | Gestion de la table ARP du noyau|
| basename | Nom du fichier sans l'extension|
| bashdb | Debugger pour bash|
| bg/fg | Mettre en fond un processus (lien avec jobs)|
| builtins | Fonction de base de bash|
| crontab | Tache planifiée|
| dd | Copie generique|
| dmesg | Message du kernel|
| egrep | grep -E|
| fgrep | grep -F|
| find | Trouver des fichiers|
| fmt | Formatter un texte|
| fuser | Processus utilisant un fichier|
| getopt(s) | Prendre les arguments de la ligne de commande|
| hexdump | |
| hier | Contient une description de l'organisation de l'arborescence Unix|
| hostname | Nom de l'hôte|
| iconv | Convertir l'encodage d'un fichier|
| ifconfig | Configuration du reseau|
| init | Niveau d'execution (init 0 -> shutdown)|
| ipcs | Utilisation des ressources IPC System V|
| jobs | Liste des jobs en cours (A voir de plus près)|
| join | Joindre des fichiers triés|
| killall | Envoyer un signal a tous les processus de meme nom|
| ldconfig | Valider les bibliothèques dynamiques|
| locate | Trouver des fichiers|
| logger | syslog|
| mail | mail tools|
| mkfifo | Tube nommés|
| mknod | Fichiers spéciaux|
| mktemp | Fichier temporaire (Stocker des mots de passe sensibles)|
| netcat | permet de faire ce que l'on veut avec des paquets TCP et UDP| 
| netstat | Statistiques reseau|
| nice | Courtoisie d'un processus|
| nm | Lire les a.out|
| nohup | Mettre un process comme indépendant du terminal|
| nslookup| permet d'avoir des infos sur un site|
| objdump | Information sur un fichier objet|
| patch | Modification de fichiers existants|
| pr | Mettre en forme pour l'impression|
| ps | Processus|
| pstree | Arbre des processus|
| regex | POSIX regular expression|
| rename | Perl tool for rename|
| renice | Changer la courtoisie d'un processus|
| rev | Inverser les lignes d'un fichier|
| route | Gestion de la table de routage|
| route | permet de voir les routes du système|
| seq | |
| setuid | Id des processus|
| socklist | Liste des sockets actives|
| sort | Trier les lignes d'un fichier texte|
| source | |
| split | Decouper un fichier en plusieurs lignes|
| squid | Pour monter un proxy|
| stty | Configuration du terminal|
| tcpdump | Information sur le reseau|
| tcpdump | output PCAP|
| tr | Eliminer ou convertir des lettres d'un texte|
| traceroute | Itineraire d'un paquet|
| tsort | |
| uname | Informations systèmes|
| uniq | Ote les lignes dupliquées|
| uptime | Uptime|
| vmstat | |
| w | Qui est connecté sur la machine|
| wc | |
| wodim | Graveur en ligne de commande|
| xargs | Ligne de commandes|
| xxd | |

Kernel module:
--------------

|Command |Meaning |
|:-----: |------- |
|depmod| Verification des dependances|
|insmod| Insertion d'un module dans le noyau|
|lsmod| Liste des modules employés|
|modinfo| Information sur un fichier module|
|modprobe| Chargement gérant les dépendances|
|rmmod| Suppression d'un fichier dans le noyau|
|sysctl| Paramètres du noyau (possible de les reconfigurer a chaud)|

Tools:
-----

|Command |Meaning |
|:-----: |------- |
| ab| benchrmarking web servers|
| bc| calculator|
| cssh| visual concurrent shell|
| cut|and paste and join: data manipulation|
| dd| moving data between files|
| dmesg| boot and system error messages|
| dstat|and htop: improved system stats monitors|
| env| run a command (useful in scripts)|
| file| identify type of a file|
| hd|and bvi: dump or edit binary files|
| iconv|or uconv: conversion for text encodings|
| iftop|or nethogs: network utilization by socket or process|
| last| login history|
| ldd| dynamic library info -> Ce dont on a besoin pour lancer un executable|
| lsof| process file descriptor and socket info|
| mtr| better traceroute for network debugging|
| nc| network debugging and data transfer|
| nm| symbols from object files|
| pr| format text|
| sar| historic system stats|
| shuf| random selection of lines from a file|
| split|and csplit: splitting files|
| stat| file info|
| strace| system call debugging|
| strings| extract text from binary files|
| tac| print files in reverse|
| tr| character translation or manipulation|
