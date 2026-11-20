# Alaska — launcher Android

Projet Java Android pour autoradio F9212A, écran paysage 1024×600, minSdk 23, targetSdk 29, compileSdk 33, AGP 7.4.2, Gradle 7.5, JDK 17.

Le projet complet est fourni dans l'archive source jointe à la conversation. Le workflow GitHub Actions construit l'APK debug et publie l'artefact `Alaska-debug-apk`.

Fonctions : interface native, GPS, météo Open-Meteo, applications installées, WebView 3D hors ligne avec Three.js embarqué au build, et métadonnées média via NotificationListenerService.

Limites : le modèle Golf est procédural stylisé; le GLB de 91 Mo n'est pas intégré car il dépasse le budget de 30 000 triangles et textures 1024 px. La signature stable release, un vrai économiseur d'écran et les tests matériels restent à finaliser. L'APK debug ne convient pas à la vente.

Personnalisation : `app/src/main/java/fr/alaska/launcher/ClientConfig.java` dans l'archive source.

Build : GitHub → Actions → Construire Alaska APK → Run workflow → télécharger `Alaska-debug-apk`.