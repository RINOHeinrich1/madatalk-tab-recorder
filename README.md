# Enregistreur d'onglet

Petit enregistreur vidéo fait maison : capture un onglet, une fenêtre ou tout
l'écran via `getDisplayMedia`, puis permet de télécharger la vidéo en `.webm`.

- 100 % côté navigateur (aucun fichier envoyé sur un serveur)
- Audio d'onglet optionnel (case « Partager l'audio de l'onglet »)
- Prévisualisation pendant et après l'enregistrement
- Arrêt automatique si le partage est coupé depuis le bandeau du navigateur
- Nécessite un contexte sécurisé (HTTPS ou localhost)

## Utilisation

Ouvrir `index.html` (ou la version publiée), cliquer sur
« Démarrer l'enregistrement », choisir l'onglet, puis « Télécharger la vidéo ».

Format produit : WebM (VP9/VP8 + Opus selon le navigateur), lisible par Chrome,
VLC et la plupart des outils de montage.

## Déploiement local

```bash
python3 -m http.server 8080
# puis http://localhost:8080
```
