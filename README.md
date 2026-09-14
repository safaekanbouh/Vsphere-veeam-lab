# Vsphere-veeam-lab
Lab de virtualisation d'entreprise VMware vSphere (ESXi, vCenter, iSCSI) + déploiement Veeam Backup &amp; Replication

# 🖥️ vSphere & Veeam Lab

Lab personnel de virtualisation d'entreprise reproduisant une infrastructure VMware vSphere complète, avec déploiement d'une solution de sauvegarde Veeam Backup & Replication.

## 🎯 Objectif du projet

Concevoir, déployer et administrer une infrastructure de virtualisation fiable, sécurisée et hautement disponible, basée sur des outils standards de l'industrie (VMware vSphere), dans un environnement de lab personnel (ressources matérielles limitées, virtualisation imbriquée).

## 🏗️ Architecture mise en place

- **Hyperviseurs ESXi** (VMware ESXi, hyperviseur bare-metal)
- **vCenter Server (VCSA)** — gestion centralisée des hôtes ESXi
- **Cluster HA/DRS** avec vMotion (migration à chaud des VMs)
- **Stockage partagé iSCSI** (mini-SAN via targetcli, datastore VMFS partagé entre hôtes)
- **Veeam Backup & Replication** — sauvegarde et restauration d'entreprise

## 🔧 Ce qui a été réalisé

- Déploiement et configuration de deux hôtes ESXi
- Configuration du stockage partagé iSCSI (LUN, datastore VMFS multi-hôtes)
- Déploiement de vCenter Server (VCSA)
- Mise en place d'un cluster avec HA, DRS et vMotion validés
- Déploiement de Veeam Backup & Replication (serveur Veeam sous Windows Server 2022)
- Configuration d'un repository de sauvegarde
- Jobs de sauvegarde et tests de restauration (fichiers)

## 📚 Modules couverts (rapport théorique + pratique)

1. Pourquoi la virtualisation existe (hyperviseurs Type 1 vs Type 2)
2. Architecture ESXi (VMkernel, DCUI, Host Client)
3. vCenter & gestion centralisée
4. Clustering, HA, DRS
5. Stockage pour la virtualisation (iSCSI, VMFS)
6. Réseau dans vSphere (vSwitches, port groups)
7. Gestion du cycle de vie des VMs (snapshots, templates)

## 🛠️ Outils utilisés

VMware ESXi · vCenter Server · VMware Workstation (lab imbriqué) · Veeam Backup & Replication · Windows Server 2022 · Linux (Storage-VM, targetcli)
