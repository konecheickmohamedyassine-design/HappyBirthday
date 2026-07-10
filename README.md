# Happy Birthday App 

## Description

**Happy Birthday App** est une application Android développée avec **Kotlin** et **Jetpack Compose**. Elle affiche une carte d'anniversaire composée d'une image de fond et d'un message personnalisé superposé.

Ce projet a pour objectif de découvrir les concepts fondamentaux de Jetpack Compose, notamment la création de composants d'interface, la gestion des mises en page et l'application d'un thème Material Design 3.

---

## Fonctionnalités

* Affichage d'une image de fond.
* Superposition d'un message d'anniversaire.
* Signature de l'expéditeur.
* Interface développée entièrement avec Jetpack Compose.
* Utilisation de Material Design 3.
* Aperçu en temps réel grâce à `@Preview`.

---

## Technologies utilisées

* **Langage :** Kotlin
* **Framework UI :** Jetpack Compose
* **Architecture :** Android Compose
* **Design :** Material Design 3
* **IDE recommandé :** Android Studio

---

## Structure du projet

```
app/
│
├── java/com/example/happybirthday/
│   ├── MainActivity.kt
│   └── ui/theme/
│
├── res/
│   ├── drawable/
│   │   └── androidparty.png
│   └── values/
│
└── AndroidManifest.xml
```

---

## Description des principaux composants

### MainActivity

Point d'entrée de l'application.

Elle :

* initialise l'interface utilisateur ;
* applique le thème Material Design ;
* affiche la carte d'anniversaire.

---

### GreetingText()

Composable chargé d'afficher :

* le message principal ;
* la signature de l'expéditeur.

Les éléments sont organisés verticalement grâce au composant `Column`.

---

### GreetingImage()

Composable responsable de :

* charger l'image depuis `res/drawable`;
* afficher cette image comme arrière-plan ;
* superposer le texte grâce au composant `Box`.

---

### BirthdayCardPreview()

Permet de visualiser rapidement l'interface dans Android Studio sans lancer l'application.

---


## Personnalisation

Vous pouvez facilement modifier :

* le message d'anniversaire ;
* le nom de l'expéditeur ;
* l'image de fond (`androidparty.png`) ;
* les couleurs du thème ;
* la taille et le style du texte.

Exemple :

```kotlin
GreetingImage(
    "Joyeux anniversaire Alice !",
    "De la part de Jean"
)
```

---

## Auteur

KONE CHEICK MOHAMED YASSINE

---

## Licence

Ce projet est distribué à des fins pédagogiques. Vous pouvez le modifier et le réutiliser librement pour vos travaux d'apprentissage.
