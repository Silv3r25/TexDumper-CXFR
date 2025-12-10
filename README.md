# 📸 TexDumper CXFR

**TexDumper CXFR** est un outil utilitaire pour *CarX Drift Racing Online* conçu pour extraire les textures de n'importe quelle map (Standard ou Workshop). C'est le compagnon idéal pour les moddeurs utilisant **TexLoader CXFR** afin de créer des packs de textures personnalisés.

<img width="1549" height="912" alt="Capture d’écran 2025-12-08 202450" src="https://github.com/user-attachments/assets/9a59c3c2-e588-437c-b5f1-2b83b4f8f5b2" />

## 🚀 Fonctionnalités Clés

* **Extraction Intelligente :** Scanne la scène entière pour trouver **tous** les types de textures, pas seulement les principales.
    * *Types supportés :* MainTex, Albedo, Normal Maps, Metallic/Specular, Emissions, Detail Masks.
    * *Environnement :* Extrait les Skyboxes et les couches de Terrain (Splats, Diffuse, Normal).
* **Compatible Workshop :** Détecte automatiquement les IDs des maps Steam Workshop (ex: `3078997877`) et crée des dossiers dédiés pour garder vos dumps organisés.
* **Intégration Parfaite :** S'ouvre aux côtés de TexLoader avec le raccourci `Ctrl + P`. Reprend le style visuel "Deep Dark" pour une expérience cohérente.
* **Performance :** Utilise la technologie "Time Slicing" pour dumper des milliers de textures sans geler le jeu (Zéro Freeze).
* **Anti-Duplication :** Système de hachage intelligent pour éviter d'exporter la même texture plusieurs fois sous des noms différents.

## 🛠️ Installation

1.  Assurez-vous d'avoir **Kino** installé.
2.  Téléchargez `TexDumper.dll` depuis l'onglet [Releases](https://github.com/Silv3r25/TexDumper-CXFR/releases/tag/v1.0.0).
3.  Placez le fichier dans votre dossier `kino/mods/`.
4.  Lancez le jeu !

## 📖 Comment l'utiliser

1.  Chargez une map (Officielle ou Workshop).
2.  Appuyez sur `Ctrl + P` pour ouvrir le menu (il apparaîtra sur la droite de l'écran).
3.  Cliquez sur **📂 OPEN FOLDER** pour voir où les textures seront sauvegardées.
4.  Cliquez sur **📥 DUMP TEXTURES** pour lancer le processus.
    * *La barre de progression affichera le statut.*
    * *Les textures sont sauvegardées dans :* `kino/mods/TexLoaderFix/Dumps/[NomMap_ID]/`

## ⚙️ Infos Techniques

* **Format de sortie :** `.png` (Non compressé)
* **Dépendances :** Peut fonctionner seul, mais conçu pour s'intégrer à *TexLoaderFix*.
* **Technologie RenderTexture :** Utilise le GPU (blitting) pour extraire même les textures illisibles/compressées que les dumpers classiques ne peuvent pas toucher.

---
*Créé par S!LVER*
