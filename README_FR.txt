BMS GÉNÉRATEUR DE LICENCE — PROJET ANDROID

Ce dossier est le projet source Android Studio destiné à produire l'APK.
Ce n'est PAS encore un fichier APK installable.

CONTENU
- app/src/main/assets/index.html : interface et générateur HTML.
- MainActivity.kt : écran Android qui ouvre l'application intégrée.
- Aucun accès Internet n'est demandé par cette application.

COMPILATION
1. Sur un ordinateur, installer Android Studio (version récente) et le JDK 17.
2. Décompresser BMS_Generateur_Android.zip.
3. Dans Android Studio, choisir Open et sélectionner le dossier BMS_Generateur_Android.
4. Laisser Android Studio synchroniser Gradle et installer les composants SDK demandés.
5. Ouvrir Build > Build Bundle(s) / APK(s) > Build APK(s).
6. L'APK de test sera dans app/build/outputs/apk/debug/app-debug.apk.

IMPORTANT — SÉCURITÉ
Le fichier HTML intégré contient la clé privée qui signe les licences. Garder le projet et l'APK strictement confidentiels. Ne pas envoyer l'APK aux établissements : seul le code de licence généré doit leur être communiqué.

À TESTER AVANT USAGE RÉEL
- Vérifier que la signature WebCrypto fonctionne dans le WebView du téléphone ciblé.
- Générer un code et vérifier son acceptation par la version actuelle de BMS ÉVALUATION.
- Vérifier que le suivi local reste présent après fermeture et réouverture.

Cette version garde le registre sur l'appareil administrateur. Elle ne fournit pas de synchronisation ni de révocation à distance.
