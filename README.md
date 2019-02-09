# Mirror

## Introduction
Cette application vous permet d'héberger un mirroir Linux Debian.

## Utilisation
L'application est composée de 2 containers : 
* le premier easylinux/mirror:apt est basé sur une Debian 9.7. Son role est la mise à jour du dépôt.
* le second easylinux/mirror:web est basé sur une Alpine 3.9. Son rôle est de servir les paquets.

## Persistance
Un dépôt contient un grand nombre de données et doit être disponible en permanence. Il est nécessaire de créer un espace disque sur un volume à cet effet.
Le volume contiendra un fichier 'mirror.list'. C'est ce fichier qui donne les directives à apt-mirror.

