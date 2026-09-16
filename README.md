# Microsoft Presales Architect — AppStudio Edition 1.0

Version Android classique **Java + XML**, conçue pour être plus simple à importer et compiler dans un IDE Android mobile tel qu'AppStudio.

## Fonctions incluses

1. Windows Server licensing
2. SQL Server licensing
3. Microsoft 365 BOM review
4. Copilot Studio sizing
5. Keepit presales
6. BitTitan MigrationWiz sizing
7. CSP Price List search
8. CSP Price List compare
9. Partner Center price-sheet request builder
10. Presales Technical Brief

## Choix techniques

- Java 17
- XML layouts
- Android SDK classique
- Pas de Jetpack Compose
- Pas de bibliothèque AndroidX requise
- Pas de dépendance tierce
- minSdk 23
- target/compile SDK 34

Cette structure maximise la compatibilité avec les IDE/builders Android mobiles.

## Import dans AppStudio

1. Décompresse le ZIP dans le stockage du téléphone.
2. Dans AppStudio, utilise l'option d'ouverture/import d'un projet existant.
3. Sélectionne le dossier racine `microsoft-presales-architect-appstudio-1.0`.
4. Laisse AppStudio synchroniser le projet Gradle.
5. Lance **Build APK / Run** selon les options disponibles dans ta version d'AppStudio.
6. Installe l'APK généré.

Si AppStudio demande la version Java/JDK, utilise **JDK 17**.

## Si AppStudio refuse AGP 8.2.2

Certains builders mobiles embarquent une version Gradle/AGP précise. Dans ce cas,
il suffit généralement d'aligner les deux versions dans `build.gradle`.
Le code Java/XML de l'application ne dépend pas d'AGP 8.2.2 spécifiquement.

## CSP CSV

Les écrans `CSP Price Search` et `CSP Compare` utilisent le sélecteur de fichiers Android.
Aucune permission de stockage globale n'est nécessaire.

## Important

Les moteurs de licensing sont des assistants de calcul et de qualification.
Pour un cas client réel, valider les règles commerciales/licensing qui peuvent évoluer
dans la documentation officielle Microsoft, Keepit et BitTitan.
