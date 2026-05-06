# LAB-12-Bypass-de-la-D-tection-de-Root-Android-avec-Medusaaa
<img width="1297" height="478" alt="image" src="https://github.com/user-attachments/assets/0e77e221-a656-4b8f-ad8b-5c103e4f5bd1" />
<img width="859" height="35" alt="image" src="https://github.com/user-attachments/assets/69b0d8b9-ab8e-4707-99ca-0098da37b394" />
<img width="1919" height="1033" alt="image" src="https://github.com/user-attachments/assets/6b294341-3f7a-46d0-b36a-09264580b1fb" />
<img width="1650" height="102" alt="image" src="https://github.com/user-attachments/assets/ec009ef7-52b9-4414-9ef7-0fde8582b46b" />

# Lab : Contournement de la Détection de Root sous Android (Root Bypass)

**Auteur :** Ammar Bensliman | **École :** EMSI (École Marocaine des Sciences de l'Ingénieur)
**Niveau :** Débutant 
**Catégorie :** Sécurité Mobile / Pentesting Android

---

## Objectif du Lab
Ce projet documente, étape par étape, la méthode pour contourner les mécanismes de détection de root d'une application Android. Nous utilisons d'abord **Medusa** (un framework basé sur Frida), et nous proposons une alternative manuelle avec des scripts **Frida** purs (Plan B).

> **Avertissement Éthique :** Les techniques présentées ici sont strictement à but éducatif. Ne les utilisez que sur des applications et des appareils que vous êtes explicitement autorisé à auditer.

---

## Prérequis
* Un PC (Windows, macOS ou Linux) avec les droits administrateur.
* Python 3.8+ et `pip` installés.
* **ADB** (Android Platform Tools) configuré.
* Un appareil Android physique (ou un émulateur) rooté avec :
  * Débogage USB activé.
  * Options développeur activées.
* Le nom du package de l'application cible (ex: `com.example.rootcheck`).

---

## Étape 1 : Préparation de l'environnement (Frida & ADB)

### 1. Installation de Frida côté PC
```bash
pip install --upgrade frida frida-tools
