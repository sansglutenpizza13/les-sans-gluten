# Les Sans Gluten — site Saison 1

Site statique responsive prêt pour Firebase Hosting.

## Contenu
- `index.html` : page d’accueil, concept, personnages, carte de Léa, rubrique « Dans la vraie vie ».
- `episode-1.html` : épisode 1 complet.
- `assets/episode-01-rentree-sans-miettes.png` : illustration principale.
- `styles.css` : design desktop + mobile.
- `script.js` : menu mobile.
- `firebase.json` : configuration Firebase Hosting.

## Déploiement Firebase
1. Installer Firebase CLI : `npm install -g firebase-tools`
2. Se connecter : `firebase login`
3. Dans ce dossier : `firebase init hosting`
4. Sélectionner le projet Firebase dédié au site Les Sans Gluten.
5. Conserver `.` comme dossier public et ne pas écraser `index.html`.
6. Déployer : `firebase deploy --only hosting`
7. Dans Firebase Console > Hosting > Ajouter un domaine personnalisé, saisir votre nom de domaine et ajouter les enregistrements DNS demandés chez votre registrar.

Domaine officiel prévu : `https://lessansgluten.fr`. Les balises SEO canoniques et Open Graph du site sont configurées pour ce domaine.


## Domaine officiel
- Domaine racine : `lessansgluten.fr`
- Recommandation : faire de `https://lessansgluten.fr` l’adresse canonique et rediriger `www.lessansgluten.fr` vers le domaine racine.
- Dans Firebase Hosting, utiliser « Ajouter un domaine personnalisé » et suivre exactement les enregistrements DNS fournis par Firebase.
