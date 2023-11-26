SE4 - Virtualisation
====================

Répartition du cours
--------------------

* Administration des systèmes et réseaux 2H CTP

Module de 2H de CTP

    * Processus de boot BIOS et UEFI
    * Explication des protocoles DNS / DHCP / SSH
    * Couches OSI
    * IP / routes / VLAN / bridge
    * Firewall + OPNsense
    * LDAP
* Virtualisation 8H CTD
    * Fonctionnement d'un système d'exploitation (OS / Kernel / Bootloader) + gestionnaires de services
    * Containers et namespaces
    * Types de virtualisation + Proxmox
    * Docker
    * Stack Hashicorp (Nomad / Consul / Vault)
    * Creation d'images Deb-based et BSD-based
    * Stockage distribue + Ceph
    * Reverse proxies + Nginx + HAProxy
#### Preparation du TP
    * Login manager + Window manager
* Approche applicative des réseaux et virtualisations 14H TP
    Tout le but du TP sera de créer un OS bootable par le réseau.
    Cet OS donnera une expérience proche de celle des postes fournis par le service informatique, mais stateless
    Chaque groupe aura une VM de dev, une pour le test de l'OS et une derniere pour le pare-feu.
    Etapes:
    * Installation d'une Debian sur une VM proxmox (a la main)
    * Création d'une image Debian minimal avec juste SSH
    * Installation de Nomad et Consul via Ansible (vu avec Thomas Maurice)
    * Déploiement d'isc-dhcp-server avec une configuration dynamique définie dans Consul
    * Installation d'HAProxy en container
    * Démarrage de l'OS minimal
    * Création + déploiement d'un nouvel OS avec un window manager
    * Ajout de LDAP et d'un login manager + déploiement de l'OS
    * Ajout d'un mountpoint Ceph rbd ou CephFS ou NFS pour la session utilisateur
    * Installation d'OPNsense sur une nouvelle VM
    * Configuration et déploiement de l'OS avec le proxy transparent

# vim: set spell spelllang=fr:
