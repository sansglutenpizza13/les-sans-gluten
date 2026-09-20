# Mise en ligne de lessansgluten.fr

## 1. Créer un projet Firebase dédié
Créer un nouveau projet Firebase nommé « Les Sans Gluten ».
Utiliser Firebase Hosting classique (site statique), pas App Hosting.

## 2. Déployer le site
Depuis un terminal avec Firebase CLI :

```bash
firebase login
cd les-sans-gluten-site
firebase deploy --only hosting --project VOTRE_PROJECT_ID
```

Le dossier contient déjà `firebase.json`; ne pas relancer une initialisation qui écraserait les fichiers.

## 3. Connecter le domaine
Dans Firebase Console > Hosting > Ajouter un domaine personnalisé :

- saisir `lessansgluten.fr`
- conserver `lessansgluten.fr` comme domaine principal
- ajouter aussi `www.lessansgluten.fr` et le rediriger vers `lessansgluten.fr`

Firebase affiche les enregistrements DNS exacts à créer chez le registrar. Les recopier à l’identique.

## 4. SSL
Firebase crée automatiquement le certificat HTTPS. Le statut peut rester « En attente » pendant la propagation DNS.

## 5. Adresse finale
https://lessansgluten.fr
