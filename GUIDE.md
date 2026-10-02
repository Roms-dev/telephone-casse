# Téléphone Cassé : mise en ligne

Le fichier `index.html` contient déjà l'URL et la clé de ton projet Supabase `pas-picasso`.
Tu peux réutiliser CE MÊME projet Supabase : il n'y a rien à créer ni à modifier dedans
(les deux jeux utilisent des canaux différents et ne se mélangent pas).

## 1. GitHub : un nouveau dépôt
1. Sur github.com, clique sur **+** puis **New repository** (Nouveau dépôt).
2. Nom : `telephone-casse`, puis **Create repository**.
3. Clique sur le lien **téléchargez un fichier existant** (uploading an existing file).
4. Glisse le fichier `index.html` (pas le dossier, pas le zip) dans la zone.
5. Clique sur **Commit changes**.
6. Vérifie que `index.html` apparaît à la racine du dépôt.

## 2. Vercel : un nouveau projet
1. Sur vercel.com, clique sur **Add New...** puis **Project**.
2. À côté de `telephone-casse`, clique sur **Import**.
3. Ne change aucun réglage (Framework Preset : Other), puis **Deploy**.
4. Après environ 30 secondes, ouvre l'adresse obtenue (du type `telephone-casse.vercel.app`).

## 3. Tester
1. Ouvre l'adresse dans 3 onglets (le jeu demande 3 joueurs minimum).
2. Onglet 1 : pseudo, puis **Créer une salle**. Un code à 4 lettres apparaît.
3. Onglets 2 et 3 : pseudo, code, puis **Go**.
4. Onglet 1 : **Lancer la partie**.

## Règles et conseils
- Chaque joueur écrit une phrase, puis elle passe de main en main : dessinée, décrite, redessinée...
- À la fin, le créateur de la salle dévoile les albums avec le bouton **Suite** (idéal sur le vidéoprojecteur).
- Le créateur fait tourner la partie : il garde son onglet ouvert. S'il le ferme, la partie s'arrête.
- De 3 à 12 joueurs par salle. Une partie démarrée n'accepte plus de nouveaux joueurs.
- Si un joueur ne répond pas à temps, le jeu complète à sa place (phrase au hasard, page blanche...).

## Si ça ne marche pas
| Problème | Solution |
|---|---|
| « Connexion impossible » | Remplace la clé `sb_publishable_...` par la clé `anon` (commence par `eyJ`) de l'onglet Legacy API keys de Supabase, directement dans `index.html` sur GitHub (crayon, puis Commit changes). |
| « Salle introuvable » | Code faux, ou le créateur a fermé sa page. |
| « La partie a déjà commencé » | Attends la fin, ou demande au créateur de recréer une salle. |
| Page blanche sur Vercel | `index.html` doit être à la racine du dépôt, avec ce nom exact. |
