# Guide de mise en ligne sur GitHub Pages

Ce guide explique comment publier le site sans écrire une seule ligne de commande.
Comptez une dizaine de minutes. Le résultat est un site public et gratuit.

---

## Ce que contient le dossier

```
site/
├── index.html                    ← page d'accueil (présentation du projet)
├── outil.html                    ← questionnaire interactif de diagnostic
├── .nojekyll                     ← fichier technique, à conserver
├── README.md                     ← description du dépôt
└── assets/
    ├── css/style.css             ← mise en forme du site
    ├── img/                      ← les 4 figures
    └── doc/                      ← la fiche de projet en PDF et en Word
```

**Tous ces fichiers doivent rester ensemble et conserver leurs noms.**
Si vous renommez `index.html`, la page d'accueil ne s'affichera plus.

---

## Étape 1 — Créer un compte GitHub

Rendez-vous sur **github.com** et créez un compte gratuit si vous n'en avez pas.
Notez bien votre nom d'utilisateur : il apparaîtra dans l'adresse du site.

---

## Étape 2 — Créer le dépôt

1. Cliquez sur le **+** en haut à droite, puis sur **New repository**.
2. **Repository name** : `diagnostic-aviaire` (ce nom apparaîtra dans l'adresse du site).
3. Cochez **Public** — c'est obligatoire pour la publication gratuite.
4. Ne cochez **rien d'autre** (ni README, ni .gitignore, ni licence).
5. Cliquez sur **Create repository**.

---

## Étape 3 — Envoyer les fichiers

Sur la page du dépôt qui vient de s'ouvrir :

1. Cliquez sur le lien **uploading an existing file**.
2. Ouvrez le dossier `site` sur votre ordinateur.
3. Sélectionnez **le contenu du dossier**, pas le dossier lui-même :
   `index.html`, `outil.html`, `README.md`, `.nojekyll` et le dossier `assets`.
4. Faites-les glisser dans la zone de dépôt de la page GitHub.
5. Attendez la fin du transfert, puis cliquez sur **Commit changes** en bas.

> **Si le fichier `.nojekyll` n'apparaît pas** dans votre explorateur : sous Windows,
> activez « Éléments masqués » dans l'onglet Affichage ; sous Mac, appuyez sur
> `Cmd + Maj + .` dans le Finder. Ce fichier n'est pas indispensable, mais il évite
> certains problèmes d'affichage.

---

## Étape 4 — Activer la publication

1. Dans le dépôt, ouvrez l'onglet **Settings** (en haut à droite).
2. Dans le menu de gauche, cliquez sur **Pages**.
3. Sous **Source**, choisissez **Deploy from a branch**.
4. Sous **Branch**, sélectionnez **main**, puis **/ (root)**, et cliquez sur **Save**.
5. Rechargez la page au bout d'une minute : l'adresse du site s'affiche en haut.

L'adresse aura cette forme :

```
https://VOTRE-NOM-UTILISATEUR.github.io/diagnostic-aviaire/
```

La première mise en ligne demande **entre 1 et 5 minutes**. Si la page affiche
une erreur 404, patientez et rechargez.

---

## Étape 5 — Vérifier

Ouvrez l'adresse et contrôlez trois points :

- la page d'accueil s'affiche avec les quatre figures ;
- le bouton **Lancer l'outil de diagnostic** ouvre bien le questionnaire ;
- le bouton **Télécharger la fiche (PDF)** ouvre le document.

Testez aussi depuis un téléphone : le site est prévu pour s'adapter aux petits écrans.

---

## Modifier le site plus tard

Pour changer un texte : ouvrez le fichier concerné directement sur GitHub, cliquez
sur l'icône **crayon**, modifiez, puis **Commit changes**. Le site se met à jour
automatiquement en une à deux minutes.

Pour remplacer une figure : envoyez la nouvelle image dans `assets/img/` **en
gardant exactement le même nom de fichier**.

---

## Adresse personnalisée (facultatif)

Si vous achetez un nom de domaine, indiquez-le dans **Settings → Pages → Custom
domain**, puis ajoutez chez votre hébergeur un enregistrement CNAME pointant vers
`VOTRE-NOM-UTILISATEUR.github.io`. Cochez ensuite **Enforce HTTPS**.

---

## Points d'attention

**Ce site est une vitrine, pas encore l'application complète.** Le questionnaire
fonctionne entièrement dans le navigateur du visiteur : aucune donnée n'est
enregistrée, aucun compte n'existe, et rien n'est transmis à un serveur.

Les modules qui supposent un serveur — comptes utilisateurs, historique des cas,
VetBot, VetoCam, carte des maladies — ne peuvent pas fonctionner sur GitHub Pages,
qui n'héberge que des pages statiques. Ils nécessiteront un hébergement avec base
de données lorsque vous passerez à la version complète.

**Mentionnez toujours** que l'outil est une aide à la décision et que la
responsabilité diagnostique reste au vétérinaire — cette mention figure déjà dans
le questionnaire et sur la page d'accueil.
