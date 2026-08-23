# Plateforme intelligente d'aide au diagnostic vétérinaire aviaire

Outil d'aide à la décision pour le **diagnostic différentiel des affections
respiratoires en élevage avicole**, calibré sur l'épidémiologie marocaine.

Projet réalisé par **EL ORCH Youssef**
Institut Agronomique et Vétérinaire Hassan II — Département de Pathologie et Santé
Publique Vétérinaire — Année universitaire 2025-2026.

---

## Contenu

| Fichier | Rôle |
|---|---|
| `index.html` | Page de présentation du projet |
| `outil.html` | Questionnaire interactif de diagnostic différentiel |
| `assets/css/style.css` | Mise en forme du site |
| `assets/img/` | Figures explicatives |
| `assets/doc/` | Fiche de projet au format PDF et Word |
| `GUIDE_DEPLOIEMENT.md` | Marche à suivre pour publier le site |

---

## Le questionnaire

Le module de diagnostic repose sur un **arbre décisionnel pondéré** portant sur
17 hypothèses respiratoires et 14 questions. Chaque réponse renforce, affaiblit
ou élimine une hypothèse, et le classement se met à jour en temps réel.

Deux sécurités sont intégrées :

- une **alerte automatique** dès que les réponses évoquent une influenza aviaire
  hautement pathogène ou une maladie de Newcastle vélogène, avec interruption du
  questionnaire et rappel de la conduite réglementaire ;
- un **amortissement volontaire des scores**, afin de ne jamais afficher de fausse
  certitude sur des données déclaratives.

Le questionnaire fonctionne entièrement dans le navigateur : aucune donnée n'est
enregistrée ni transmise.

---

## Avertissement

Cet outil **aide à la décision, il ne pose pas de diagnostic**. Il hiérarchise des
hypothèses et oriente les prélèvements à réaliser. La décision finale et la
responsabilité qui l'accompagne restent entières et exclusives au médecin
vétérinaire.

---

## État du projet

La version publiée ici est une **vitrine avec un module de diagnostic
fonctionnel**. Les modules VetBot, VetoCam, la carte des maladies, les comptes
utilisateurs et l'historique des cas nécessitent un hébergement avec base de
données et ne sont pas inclus dans cette version statique.
