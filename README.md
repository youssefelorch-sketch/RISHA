# Outil de diagnostic différentiel — Affections respiratoires aviaires

Questionnaire guidé d'aide au diagnostic différentiel des affections respiratoires
en élevage avicole, calibré sur l'épidémiologie marocaine.

Réalisé par **EL ORCH Youssef** — Institut Agronomique et Vétérinaire Hassan II.

---

## Principe

L'outil repose sur un **arbre décisionnel pondéré** portant sur **17 hypothèses
respiratoires** et **14 questions**. Chaque réponse renforce, affaiblit ou élimine
une hypothèse, et le classement se met à jour en temps réel avec la liste des
maladies écartées et le motif de leur élimination.

Deux sécurités sont intégrées :

- une **alerte automatique** dès que les réponses évoquent une influenza aviaire
  hautement pathogène ou une maladie de Newcastle vélogène, avec interruption du
  questionnaire et rappel de la conduite réglementaire à tenir ;
- un **amortissement volontaire des scores**, afin de ne jamais afficher de fausse
  certitude sur des données déclaratives.

À la fin, l'outil produit une synthèse imprimable indiquant les trois hypothèses
principales, les tests de confirmation à demander et la conduite à tenir.

---

## Fonctionnement technique

Le questionnaire fonctionne **entièrement dans le navigateur du visiteur**.
Aucune donnée n'est enregistrée, aucun compte n'est requis et rien n'est transmis
à un serveur. Le fichier `index.html` est autonome : il contient la mise en forme
et la logique de calcul.

---

## Avertissement

Cet outil **aide à la décision, il ne pose pas de diagnostic**. Il hiérarchise des
hypothèses et oriente les prélèvements à réaliser. La confirmation repose sur
l'autopsie de 5 à 10 sujets et sur le laboratoire. La décision finale et la
responsabilité qui l'accompagne restent entières et exclusives au médecin
vétérinaire.

Certaines maladies de la liste sont à déclaration obligatoire : en cas d'alerte,
les services vétérinaires officiels doivent être contactés sans délai.
