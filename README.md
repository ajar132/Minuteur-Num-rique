# Minuteur Numérique Programmable avec Arduino ⏲️

## 📌 Présentation du Projet
Ce projet a été réalisé dans le cadre du module **Électronique Analogique** durant ma 2ème année à l'EMSI. L'objectif est de concevoir un minuteur autonome capable de gérer un compte à rebours personnalisable par l'utilisateur avec une alerte sonore finale.

Le projet met l'accent sur la gestion précise du temps en programmation embarquée et l'optimisation de l'interface utilisateur (HMI).

## 🚀 Fonctionnalités
- **Réglage manuel** : Configuration des minutes et des secondes via des boutons-poussoirs.
- **Affichage LCD** : Interface claire utilisant un écran LCD 16x2 avec communication I2C.
- **Gestion intelligente du temps** : Utilisation de la fonction `millis()` pour un code non-bloquant.
- **Fiabilité logicielle** : Algorithme d'anti-rebond (debounce) intégré pour une lecture précise des entrées.
- **Alerte Sonore** : Activation d'un buzzer à la fin du décompte.

## 🛠️ Matériel Utilisé (Hardware)
- **Microcontrôleur** : Arduino Uno (ATmega328P)
- **Affichage** : Écran LCD 16x2 avec module I2C
- **Entrées** : 4 Boutons-poussoirs (Start, Reset, Min+, Sec+)
- **Sortie sonore** : 1 Buzzer piézoélectrique
- **Divers** : Résistances de tirage, Breadboard et câbles de liaison

## 💻 Architecture Logicielle
Le code source est structuré pour maximiser la réactivité du système :
- **Communication I2C** : Réduction du nombre de fils nécessaires pour l'affichage.
- **Logique Non-Bloquante** : Contrairement à l'utilisation de `delay()`, l'approche par `millis()` permet au microcontrôleur de rester à l'écoute des interruptions utilisateurs (comme le bouton Reset) même pendant le décompte.
- **Traitement Anti-rebond** : Filtrage logiciel des signaux parasites lors de l'appui sur les boutons.

## 📸 Schéma et Simulation
*(Conseil : Ajoute ici une image de ta simulation ou de ton circuit réel)*
![Schéma du circuit](Lien_vers_ton_image_ici)

## 📂 Structure du Dépôt
- `/src` : Contient le code source `.ino` pour Arduino.
- `/docs` : Contient le rapport de projet complet (PDF).
- `/img` : Captures d'écran de la simulation et photos du montage.

## ✍️ Auteurs
- **El Mahdi Bakirou** - [Ton profil GitHub](https://github.com/ton-username)
- **Ziad Elyousfi**

---
Projet réalisé dans un cadre académique (EMSI Casablanca, 2024-2025).
