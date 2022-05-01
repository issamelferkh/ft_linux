# ft_linux
Buiild a basic, but functional linux distribution.

## Goals
- Build a Linux Kernel
- Install some binaries (See the list below)
- Implement a filesystem hierarchy compliant with the [standards](https://refspecs.linuxfoundation.org/FHS_3.0/fhs/index.html)
- Connect to the Internet

## Helps
Linux Device Drivers
LDD Book: https://lwn.net/Kernel/LDD3/
LDD3 Example Code Updated: https://github.com/martinezjavier/ldd3

# Linux From Scratch - Version 8.0
## Preface
### Architectures cible de LFS
- les processeurs AMD/Intel x86 (32 bits) et x86_64 (64 bits)
- le prérequis principal est la présence d'un système installée (Ubuntu, Red Hat/Fedora, 
- vous pouvez installer et utiliser un système 32 bits en tant que système hôte sur un système AMD/Intel 64 bits.

### Raison de la présence des paquets dans le livre
• Acl (2.2.52)
• Attr (2.4.47)
• Autoconf (2.69)
• Automake (1.15)
• Bash (4.3.30)
• Bc (1.06.95)
• Binutils (2.25.1)
• Bison (3.0.4)
• Bzip2 (1.0.6)
• Check (0.10.0)
• Coreutils (8.24)
• DejaGNU (1.5.3)
• Diffutils (3.3)
• Eudev (3.1.2)
• E2fsprogs (1.42.13)
• Expat (2.1.0)
• Expect (5.45)
• File (5.24)
• Findutils (4.4.2)
• Flex (2.5.39)
• Gawk (4.1.3)
• GCC (5.2.0)
• GDBM (1.11)
• Gettext (0.19.5.1)
• Glibc (2.22)
• GMP (6.0.0a)
• Gperf (3.0.4)
• Grep (2.21)
• Groff (1.22.3)
• GRUB (2.02 beta2)
• Gzip (1.6)
• Iana-Etc (2.30)
• Inetutils (1.9.4)
• Intltool (0.51.0)
• IPRoute2 (4.2.0)
• Kbd (2.0.3)
• Kmod (21)
• Less (458)
• Libcap (2.24)
• Libpipeline (1.4.1)
• Libtool (2.4.6)
• M4 (1.4.17)
• Make (4.1)
• Man-DB (2.7.2)
• Man-pages (4.02)
• MPC (1.0.3)
• MPFR (3.1.3)
• Ncurses (6.0)
• Patch (2.7.5)
• Perl (5.22.0)
• Pkg-config (0.28)
• Procps (3.3.11)
• Psmisc (22.21)
• Readline (6.3)
• Sed (4.2.2)
• Shadow (4.2.1)
• Sysklogd (1.5.1)
• Sysvinit (2.88dsf)
• Tar (1.28)
• Tcl (8.6.4)
• Texinfo (6.0)
• Time Zone Data (2015f)
• Udev-lfs Tarball (udev-lfs-20140408)
• Util-linux (2.27)
• Vim (7.4)
• XML::Parser (2.44)
• Xz Utils (5.2.1)
• Zlib (1.2.8)

Acl: Ce paquet contient des outils d'administration des listes de Contrôle d'accès, utilisées pour définir plus finement les droits d'accès de votre choix pour les fichiers et les répertoires.

Attr: Ce paquet contient des programmes d'administration des attributs étendus sur les objets d'un système de fichiers.

Autoconf: Le paquet Autoconf contient des programmes produisant des scripts shell qui configurent automatiquement le code source à partir du modèle fourni par le développeur. Il est souvent requis pour reconstruire un paquet après une mise à jour des procédures de construction.

Automake: Ce paquet contient des programmes pour générer des Makefile à partir d'un modèle. Il est souvent requis pour reconstruire un paquet après des mises à jour des procédures de construction.

Bash: Ce paquet satisfait une exigence du coeur de la LSB pour fournir une interface Bourne Shell au système. Il a été choisi parmi d'autres shells du fait de son utilisation répandue et de ses fonctionnalités étendues au-delà des fonctions d'un shell de base.

Bc: Ce paquet fournit un langage de traitement numérique à précision arbitraire. Il satisfait une exigence utilisée pour la construction du noyau Linux.

Binutils: Ce paquet contient un éditeur de liens, un assembleur et d'autres outils de gestion des fichiers objets. Les programmes de ce paquet sont nécessaires pour compiler la plupart des paquets d'un système LFS et allant au-delà.

Bison: Ce paquet contient la version GNU de yacc (Yet Another Compiler Compiler, encore un nouveau compilateur) requis pour construire plusieurs autres programmes de LFS.

Bzip2: Ce paquet contient des programmes de compression et de décompression de fichiers. Il est nécessaire pour décompresser plusieurs paquets de LFS.

Check: Ce paquet contient une base de tests pour d'autres programmes. On ne l'installe que dans la chaîne d'outils temporaire.

Coreutils: Ce paquet contient un certain nombre de paquets essentiels pour visualiser et manipuler des fichiers et des répertoires. Ces programmes sont nécessaires pour la gestion de fichiers en ligne de commande et ils sont nécessaires pour les procédures d'installation de chaque paquet de LFS.

DejaGNU: Ce paquet contient un environnement de travail pour tester d'autres programmes. Il n'est installé que dans la chaîne d'outils temporaires.

Diffutils: Ce paquet contient des programmes qui montrent les différences entre des fichiers et des répertoires. On peut utiliser ces programmes pour créer des correctifs et ils sont aussi utilisés dans de nombreuses procédures de construction de paquets.

E2fsprogs: Ce paquet contient les outils de gestion des systèmes de fichiers ext2, ext3 et ext4. Ce sont les systèmes de fichiers les plus courants et les plus largement testés supportés par Linux.

Eudev: Ce paquet est un gestionnaire de périphériques. Il contrôle de façon dynamique les entrées du répertoire /dev quand des périphériques sont ajoutés ou enlevés du système.

Expat: Ce paquet contient une bibliothèque d'analyse XML relativement petite. Il est exigé par le module Perl XML::Parser.

Expect: Ce paquet contient un programme pour réaliser des dialogues scriptés avec d'autres programmes interactifs. Il est souvent utilisé pour tester d'autres paquets. Il n'est installé que dans la chaîne d'outils temporaire.

File: Ce paquet contient un outil pour déterminer le type d'un ou plusieurs fichiers donnés. Quelques paquets en ont besoin pour se construire.

Findutils: Ce paquet contient des programmes pour rechercher des fichiers sur un système de fichiers. Il est utilisé dans les scripts de construction de nombreux paquets.

Flex: Ce paquet contient un outil de génération de programmes qui reconnaît des modèles de texte. C'est la version GNU du programme lex (lexical analyzer, analyseur lexical). Il est nécessaire pour construire plusieurs paquets LFS.

Gawk: Ce paquet contient des programmes de manipulation de fichiers texte. C'est la version GNU du programme awk (Aho-Weinberg-Kernighan). Il est utilisé dans les scripts de construction de nombreux autres paquets.

Gcc: Ce paquet est le Gnu Compiler Collection. Il contient les compilateurs C et C++ ainsi que d'autres qui ne sont pas construits dans LFS.

GDBM: Ce paquet contient la bibliothèque GNU Database Manager (gestionnaire de base de données GNU). Il est utilisé par un autre paquet de LFS : Man-DB.

Gettext: Ce paquet contient des outils et des bibliothèques pour l'internationalisation et la localisation de nombreux paquets.

Glibc

Le paquet contient la bibliothèque C principale. Les programmes Linux ne peuvent pas s'exécuter sans elle.

GMP

Ce paquet contient des bibliothèques mathématiques qui fournissent des fonctions utiles pour de l'arithmétique en précision arbitraire. Il est nécessaire pour construire Gcc.

Gperf

Ce paquet contient un programme qui génère une fonction de hachage parfaite à partir d'un trousseau. Il est exigé par Eudev.

Grep

Ce paquet contient des programmes de recherche au sein de fichiers. Ces programmes sont utilisés par la plupart des scripts de construction des paquets.

Groff

Le paquet Groff contient des programmes de formatage de texte. Une des fonctions importantes de ces programmes est le formatage des pages de man.

GRUB

Ce paquet est le chargeur Grand Unified Boot. Ce n'est pas le seul chargeur de démarrage disponible, mais c'est le plus flexible.

Gzip

Ces paquets contiennent des programmes de compression et de décompression de fichiers. Il est nécessaire pour décompresser de nombreux paquets sur LFS et au-delà.

Iana-etc

Ce paquet fournit des données pour des services et des protocoles réseau. Il est nécessaire pour activer les bonnes fonctionnalités de réseau.

Inetutils

Ce paquet contient des programmes d'administration réseau de base.

Intltool

Ce paquet contient des outils pour extraire des chaînes traduisibles de fichiers sources.

IProute2

Ce paquet contient des programmes pour du réseau de base ou avancé en IPv4 et IPv6. Il a été choisi parmi les paquets d'outils réseau courants (net-tools) pour ses possibilités IPv6.

Kbd

Ce paquet contient des fichiers de tables de touches, des outils claviers pour les claviers non américains et un certain nombre de polices pour console.

Kmod

Ce paquet contient des programmes nécessaires pour administrer les modules du noyau Linux.

Less

Ce paquet contient un très bon visualiseur de texte qui permet le défilement vers le haut ou le bas lors de la visualisation d'un fichier. Il est aussi utilisé par Man-DB pour visualiser des pages de man.

Libcap

Ce paquet implémente les interfaces au niveau utilisateur avec les possibilités POSIX 1003.1e disponibles dans les noyaux Linux.

Libpipeline

Le paquet Libpipeline contient une bibliothèque pour manipuler des files (pipelines) de sous-processus de façon flexible et ommode. Il est requis par le paquet Man-DB.

Libtool

Ce paquet contient le script de support de la bibliothèque générique GNU. Il englobe la complexité de l'utilisation des bibliothèques partagées dans une interface cohérente et portable. Il est exigé par les suites de tests d'autres paquets de LFS.

Noyau Linux

Ce paquet est le système d'exploitation. C'est Linux dans l'environnement GNU/Linux.

M4

Ce paquet contient un traitement de macros textuelles générales utile en tant qu'outil de construction d'autres programmes.

Make

Ce paquet contient un programme de gestion de la construction des paquets. Il est requis par presque tous les paquets de LFS.

Man-DB

Ce paquet contient des programmes de recherche et de visualisation de pages de man. Il a été préféré au paquet man du fait d'une capacité d'internationalisation supérieure. Il fournit le programme man.

Man-pages

Ce paquet contient le contenu final des pages de man de base de Linux.

MPC

Ce paquet contient des fonctions pour le calcul de nombres complexes. Il est exigé par Gcc.

MPFR

Le paquet MPFR contient des fonctions pour des maths à précision multiple. Il est exigé par Gcc.

Ncurses

Le paquet Ncurses contient les bibliothèques de gestion des écrans type caractère, indépendant des terminaux. Il est souvent utilisé pour fournir le contrôle du curseur dans un système en menus. Il est exigé par un certain nombre de paquets de LFS.

Patch

Ce paquet contient un programme pour modifier ou créer des fichiers en appliquant un fichier de correctif créé en général par le programme diff. Il est requis par la procédure de construction de plusieurs paquets LFS.

Perl

Ce paquet est un interpréteur du langage PERL en cours d'exécution. Il est nécessaire pour l'installation et les suites de tests de plusieurs paquets LFS.

Pkg-config

Ce paquet fournit un programme pour retourner des métadonnées sur une bibliothèque ou un binaire installé.

Procps-NG

Ce paquet contient des programmes de surveillance des processus. Ces programmes sont utiles pour l'administration système et ils sont aussi utilisés par les scripts de démarrage LFS.

Psmisc

Ce paquet contient des programmes d'affichage d'informations sur les processus en cours d'exécution. Ces programmes sont utiles pour l'administration système.

Readline

Ce paquet est un ensemble de bibliothèques qui offre des fonctionnalités d'édition et d'historique de la ligne de commande. Il est utilisé par Bash.

Sed

Ce paquet permet d'entrer du texte sans l'ouvrir dans un éditeur de texte. Il est aussi requis par la plupart des scripts de configuration des paquets LFS.

Shadow

Ce paquet contient des programmes de gestion sécurisée des mots de passe.

Sysklogd

Ce paquet contient des programmes de journalisation des messages système, tels que ceux donnés par le noyau ou les processus démons lorsque se produisent des événements inhabituels.

Sysvinit

Ce paquet fournit le programme init qui est le parent de tous les autres processus du système Linux.

Tar

Ce paquet fournit des fonctionnalités d'archivage et d'extraction de potentiellement tous les paquets utilisés dans LFS.

Tcl

Ce paquet contient le Tool Command Language utilisé dans beaucoup de suites de tests des paquets LFS. Il n'est installé que dans la chaîne d'outils temporaire.

Texinfo

Ce paquet contient des programmes de lecture, d'écriture et de conversion de pages info. Il est utilisé dans les procédures d'installation de beaucoup de paquets LFS.

Util-linux

Ce paquet contient des programmes généraux. Parmi eux, se trouvent des outils de gestion des systèmes de fichiers, de consoles, de partitions et de messages.

Vim

Ce paquet contient un éditeur. Il a été choisi pour sa compatibilité avec l'éditeur vi classique et son grand nombre de fonctionnalités puissantes. Un éditeur est un choix très personnel de chaque utilisateur et vous pouvez le remplacer par n'importe quel éditeur si vous le désirez.

XML::Parser

Ce paquet est un module Perl qui interagit avec Expat.

XZ Utils

Ce paquet contient des programmes de compression et de décompression de fichiers. Il offre la compression la plus haute disponible et il est utile pour la décompression des paquets au format XZ ou LZMA.

Zlib

Ce paquet contient des routines de compression et de décompression utilisées par quelques programmes.

## Partie I - Introduction
### 1. Introduction





