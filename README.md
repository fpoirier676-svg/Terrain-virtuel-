# Mon Terrain 3D

Application web pour aménager en 3D le terrain du 70, rue Gauthier (Chicoutimi) et planifier les plantations, l'entretien et les récoltes.

## Ce qu'elle contient

- **Plan réel** : lots 5 511 832 et 5 511 834 d'après le certificat de localisation (minute 8044, 2019) et le plan cadastral.
- **Relief et arbres existants** : tirés de la tuile LiDAR du Québec 22_2685369F07 (avril 2023), calés en NAD83(SCRS) / MTM fuseau 7.
- **Bibliothèque de végétaux** adaptée au Québec (zone 3b), avec calendrier de semis, plantation, entretien, taille et récolte.
- **Projections** de croissance et de récoltes sur 15 ans, alertes d'espacement, de rotation et de rusticité.
- **Climat du site** (normales de Bagotville), journal photo et vidéo, import de modèles 3D (.glb).

## Utilisation

Ouvre `index.html` dans un navigateur, ou la version en ligne (GitHub Pages). Sur téléphone, utilise « Ajouter à l'écran d'accueil » pour l'installer comme une application. Elle fonctionne aussi hors ligne après une première visite.

## Où sont tes données

En ligne sur GitHub Pages, tes modifications (plantations, tâches, récoltes, photos) restent **dans le navigateur de l'appareil utilisé**. Pour les garder en sécurité ou passer d'un appareil à l'autre, utilise **Terrain → Exporter (.json)**, puis **Importer…** sur l'autre appareil.

## Publier ou mettre à jour le site

1. Dans le dépôt GitHub : **Settings → Pages**.
2. Sous « Build and deployment », choisis **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
3. Après une minute ou deux, le site est accessible à l'adresse indiquée sur cette page (`https://<utilisateur>.github.io/Terrain-virtuel-/`).

Toute modification poussée sur `main` met le site à jour automatiquement.

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | L'application complète (interface, scène 3D, données du terrain) |
| `manifest.webmanifest`, `icons/` | Installation sur téléphone et ordinateur |
| `sw.js` | Fonctionnement hors ligne |
