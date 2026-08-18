---
description: La description est ici.
title: Planifier une campagne
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 676
ht-degree: 1%

---

# Planifier une campagne {#schedule-campaign}

Lors du lancement d’une campagne, les utilisateurs peuvent désormais choisir le moment exact de son lancement : immédiatement, à une date et une heure futures spécifiques ou selon un planning récurrent (récurrent). Les utilisateurs peuvent également revenir ultérieurement et modifier le planning d’une campagne qui a déjà été lancée ou planifiée.

> **Changements** : auparavant, les campagnes ne pouvaient être lancées que immédiatement. Cette version ajoute une planification future unique, des planifications récurrentes et la possibilité de modifier une planification après le lancement.

## Conditions préalables

- La campagne doit être prête à être lancée (toute configuration requise est terminée).
- Aucune condition préalable requise au-delà de la possibilité de lancer une campagne.

## Fonctionnement de cette fonctionnalité

Lorsque l’utilisateur lance une campagne, il choisit l’un des trois modes de planification, puis confirme. Le planning choisi détermine le moment où la campagne commence à envoyer et, pour les campagnes récurrentes, la fréquence de répétition et le moment où elle se termine (ou si elle se termine). Une fois qu’une campagne est planifiée ou active, son planning peut être modifié à partir des paramètres de la campagne.

### Comportements clés

- Trois modes de planification sont disponibles lors du lancement : **Maintenant**, **Planifier une fois** et **Récurrent**.
- Une campagne planifiée dans le futur affiche le statut « Planifié » jusqu&#39;à l&#39;heure de début, puis passe automatiquement à « Actif ».
- Une campagne récurrente qui a démarré affiche « En direct » avec un résumé de sa périodicité (par exemple, « Hebdomadaire, le mardi, jeudi à 9 h 00 »).
- Les campagnes récurrentes peuvent être définies pour s’exécuter indéfiniment (fin « Jamais ») ou jusqu’à une date de fin spécifique. Les campagnes ponctuelles et immédiates ne comportent pas d’option de date de fin, puisqu’elles s’exécutent une seule fois.
- Les utilisateurs peuvent modifier le planning d’une campagne qui a déjà été lancée ou planifiée, à l’aide des mêmes options de planning, à partir des paramètres de la campagne.

## Comment l’utiliser

**Pour planifier une campagne au lancement :**

1. Dans la campagne, cliquez sur **Prêt pour le lancement**.
2. Dans la boîte de dialogue de lancement, choisissez une option de planification :
   - **Maintenant** — la campagne commence à envoyer immédiatement après le lancement.
   - **Planifier une fois** — choisissez une future **Date de début** (date et heure confondues).
   - **Récurrent** — choisissez une **Fréquence** (Quotidienne, Hebdomadaire ou Mensuelle) et une heure de début, puis définissez la périodicité (voir les champs ci-dessous).
3. Si Récurrent est sélectionné, choisissez si la campagne se termine **Jamais** ou **À une date**, puis choisissez une date de fin, le cas échéant.
4. Confirmez pour lancer la campagne avec le planning sélectionné.

**Pour modifier un planning existant, procédez comme suit**

1. Ouvrez la campagne et accédez à ses paramètres.
2. Recherchez la section Planning et sélectionnez la synthèse du planning actuel.
3. Mettez à jour le planning à l’aide des mêmes options que celles décrites ci-dessus.
4. Enregistrez la modification.

### Champs/paramètres de saisie

| Champ | Description | Obligatoire ? |
| --- | --- | --- |
| Mode horaire | Choix entre Maintenant, Planifier une fois ou Récurrent | Oui |
| Date de début | Date et heure de début de la campagne (mode Planifier une seule fois) | Oui, pour Planifier une fois |
| Fréquence | Quotidienne, hebdomadaire ou mensuelle (mode récurrent) | Oui, pour récurrent |
| Heure de début | Heure d’envoi par la campagne récurrente | Oui, pour récurrent |
| Jours de la semaine | Le ou les jours où la campagne se répète | Oui, pour la fréquence hebdomadaire |
| Jour du mois | Le jour du mois où la campagne se répète | Oui, pour la fréquence mensuelle |
| Terminer la campagne | Jamais, ou à une date de fin spécifique | Oui, pour récurrent |

## Légendes de l’interface utilisateur

> **Note du rédacteur technique** : des captures d’écran sont nécessaires pour les éléments suivants :

- [ ] Boîte de dialogue de lancement affichant les options Maintenant / Planifier une fois / Récurrent
- [ ] le sélecteur de date et d’heure Planifier une seule fois
- [ ] les options récurrentes : sélecteur de fréquence, bascule des jours hebdomadaires, grille mensuelle des jours du mois
- [ ] La « Fin de la campagne » Jamais / Sur un choix de date
- [ ] Le badge de statut « Planifié » sur une campagne en attente de son heure de début
- [ ] Le badge de statut « Actif » avec un résumé de la périodicité (par exemple « Hebdomadaire le mardi, jeudi à 9:00 »)
- [ ] la section Planning des paramètres de la campagne, affichant le point d’entrée de modification

## Ce que cette fonctionnalité ne fait pas

- Il ne prend pas en charge les intervalles de répétition personnalisés, tels que « toutes les 2 semaines » ou « tous les 3 jours » ; seules les fréquences standard Quotidienne, Hebdomadaire ou Mensuelle sont disponibles.
- Il ne prend pas en charge la périodicité mensuelle relative, telle que « le deuxième lundi du mois ». Seule une sélection spécifique du jour du mois est disponible pour Mensuel.
- Elle n’offre pas de date de fin pour les campagnes **Maintenant** ou **Planifier une fois** ; une date de fin n’est disponible que lorsque l’option Récurrent est sélectionnée, car les campagnes ponctuelles s’exécutent une seule fois par définition.
