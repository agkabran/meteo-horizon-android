# Météo Horizon — version web dans une application Android

Ce projet affiche **votre fichier HTML d'origine, sans modification** (`app/src/main/assets/index.html`)
dans une application Android plein écran (WebView). Android 11 minimum.

- La géolocalisation du site fonctionne : l'app demande la permission Android puis la transmet à la page.
- Le bouton Retour du téléphone fonctionne.
- Les liens externes (Open-Meteo…) s'ouvrent dans le navigateur.
- Une connexion Internet est nécessaire : la page charge Tailwind et la police Inter en ligne, en plus des données météo.

## Mettre à jour la page
Remplacez simplement `app/src/main/assets/index.html` par votre nouvelle version, puis reconstruisez l'APK.

## Obtenir l'APK

### Avec GitHub (rien à installer)
1. Créez un dépôt GitHub et envoyez-y tout le contenu de ce dossier
   (bouton « Add file › Upload files », en glissant le contenu du dossier).
2. Onglet **Actions** → le workflow « Construire l'APK » se lance (≈ 4 min).
   S'il ne démarre pas : cliquez sur le workflow puis **Run workflow**.
3. Téléchargez l'artefact **MeteoHorizon-Web-APK** → `MeteoHorizon-Web-1.0.0.apk`.

### Avec Android Studio
Ouvrez le dossier, attendez la synchronisation, puis **Build › Build APK(s)**.

## Installation
Copiez l'APK sur le téléphone, ouvrez-le et autorisez « Installer des applis inconnues ».
