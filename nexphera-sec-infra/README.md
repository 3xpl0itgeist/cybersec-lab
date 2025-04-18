# NEXPHERA – Sécurisation d'une infrastructure Linux pour PME

Ce dépôt contient un projet complet de simulation et de sécurisation d'une infrastructure informatique pour **NEXPHERA**, une entreprise fictive de services numériques spécialisée dans les solutions médicales. Le projet est structuré comme un cas réel d’intervention en cybersécurité, depuis la conception du réseau jusqu’au hardening, la surveillance et les tests de sécurité.

## Contexte

**NEXPHERA** est une PME fictive localisée à Lille, spécialisée dans le développement de solutions numériques pour le secteur de la santé. Elle propose à ses clients :
- des portails web médicaux (patients, dossiers, rendez-vous),
- des services cloud auto-hébergés,
- des formations numériques aux professionnels de santé.

L'entreprise dispose de plusieurs services internes (développement, support, formation, direction) et héberge elle-même ses applications critiques. Face à des problématiques de sécurité, elle mandate la mise en place d’un **réseau segmenté, sécurisé, surveillé**, basé sur des technologies **open-source sous Linux**.

---

## Objectifs du projet

- Concevoir une **infrastructure réseau sécurisée** (segmentée par VLAN, filtrée, auditée)
- Mettre en place des **machines virtuelles Linux durcies**
- Sécuriser les **services réseau exposés** (SSH, DNS, Apache, etc.)
- Installer un **IDS/IPS** pour détecter les intrusions
- Activer un système de **journalisation et d’audit** fiable
- Rédiger une **documentation complète** et professionnelle

---

## Technologies et outils utilisables

- **Systèmes** : Rocky Linux, Ubuntu Server
- **Virtualisation** : VirtualBox
- **Simulation réseau** : Cisco Packet Tracer
- **Pare-feu / NAT** : iptables, firewalld
- **DNS / DHCP** : Bind9, dnsmasq
- **Services web** : Apache, PHP
- **Base de données** : MariaDB
- **Surveillance système** : auditd, sysdig, journald, Falco
- **Détection d’intrusion** : Suricata (IDS)
- **Scripts / Automatisation** : Bash, fail2ban, Lynis
- **Analyse réseau** : Wireshark

---

## Structure du projet

```bash
nexphera-sec-infra/
├── README.md
├── docs/                  ← Documentation complète du projet (par étapes)
├── configs/               ← Fichiers de configuration des services
├── scripts/               ← Scripts d’automatisation et d’audit
├── assets/                ← Schémas réseau, captures d’écran, résultats
├── topology/              ← Maquette Packet Tracer + plan d’adressage
└── logs/                  ← Logs d’audit, IDS, journaux système
