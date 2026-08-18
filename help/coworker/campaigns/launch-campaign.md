---
description: La description est ici.
title: Lancement d’une campagne
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 757
ht-degree: 0%

---

# Lancement d’une campagne {#launch-campaign}

Le lancement d’une campagne est l’action qui la fait passer du statut de brouillon à celui d’envoi actif. Avant que la boîte de dialogue de lancement ne s’ouvre, Halo vérifie que la campagne est prête et bloque le lancement jusqu’à ce que la configuration requise soit terminée. La boîte de dialogue de lancement affiche un aperçu de l’e-mail et de l’audience, permet à l’utilisateur de vérifier ou de modifier le planning d’envoi en ligne et indique si le lancement a réussi. Cette section couvre l’expérience de lancement de bout en bout. Pour connaître les options de planification proposées au lancement, voir [Planifier une campagne](/help/coworker/campaigns/schedule-campaign.md).

## Conditions préalables

- La campagne doit avoir le statut Brouillon . <!-- The Launch action isn't available once a campaign is already live. -->
<!-- - The campaign must pass a readiness check: sending settings configured, at least one test email sent, and a real (non-sample) audience uploaded. -->
- [ENTRÉES NÉCESSAIRES — à confirmer auprès de l’ingénieur : certains utilisateurs peuvent voir une expérience « bientôt disponible » au lieu d’un vrai bouton de lancement, qui ne propose que de télécharger la campagne ou d’envoyer un BAT par e-mail plutôt que de lancer l’application. Confirmez ce qui détermine l’expérience obtenue par un utilisateur ou une campagne donnée.]

## Fonctionnement de cette fonctionnalité

Lorsqu’un utilisateur ou une utilisatrice lance une campagne, Halo commence par valider que la campagne est prête. Si des éléments requis sont manquants, une boîte de dialogue répertorie les éléments à corriger avant que le lancement puisse se poursuivre. Une fois la validation réussie, la boîte de dialogue de lancement affiche un aperçu de l’e-mail et de l’audience/du workflow, permet à l’utilisateur ou à l’utilisatrice de consulter ou de modifier le planning d’envoi sans quitter le flux et, pour les envois volumineux, affiche un avis de volume d’envoi estimé. La confirmation déclenche le lancement et Halo signale l’un des trois résultats suivants : lancé, déjà lancé ou en échec.

### Comportements clés

- Le lancement n’est disponible que pour les campagnes au statut Brouillon. Une campagne déjà active ne peut pas être relancée.
- Une vérification de préparation s’exécute automatiquement avant l’ouverture de la boîte de dialogue de lancement. Les problèmes non résolus bloquent le lancement et sont répertoriés avec un moyen de les résoudre.
- La boîte de dialogue de lancement affiche un aperçu d’e-mail (objet, pré-titre, expéditeur) et un aperçu d’audience/workflow.
- Le planning d’envoi peut être examiné ou modifié dans la boîte de dialogue de lancement.
- Pour les envois volumineux, la boîte de dialogue affiche une estimation de l’impact sur le volume d’envoi. [ENTRÉES NÉCESSAIRES — le libellé exact de cet avis n&#39;était pas disponible à partir du code]
- Une fois la campagne réussie, son statut passe à « Planifié » ou « Actif » (selon le planning choisi), et un message de confirmation indique que les informations sur la campagne seront disponibles dans les 2 heures.
- Si la campagne a déjà été lancée (par exemple, à partir d’un double clic), Halo affiche un message « déjà lancée » plutôt qu’une erreur.
- Si le lancement échoue, un message d’erreur s’affiche et la campagne reste dans l’état Brouillon ; l’utilisateur peut réessayer.
- Une fois qu’une campagne est arrêtée <!--(see [Stop a live campaign](./stop-live-campaign.md))-->, elle ne peut plus être relancée à partir du même enregistrement de campagne. L’arrêt est un état distinct et permanent.

## Accès

**Pour lancer une campagne, procédez comme suit**

1. Dans la campagne, cliquez sur **Lancer** (indiqué comme « Prêt à démarrer » lorsque vous êtes encore en version brouillon).
2. S’il manque quelque chose, une boîte de dialogue intitulée « Quelques éléments nécessitent encore une attention » répertorie les éléments à compléter :
   - **Configurer les paramètres d’e-mail** — les paramètres d’envoi (expéditeur/domaine) n’ont pas encore été configurés.
   - **E-mails non testés** — Envoyez au moins un e-mail de test pour tester l’e-mail avant le lancement.
   - **Audience réelle requise pour le lancement** — la campagne utilise toujours un exemple d’audience ; chargez un CSV d’audience réelle.
     Résolvez chaque élément, puis réessayez de lancer.
3. Une fois que la campagne a réussi le contrôle de préparation, la boîte de dialogue de lancement s’ouvre, affichant un aperçu de l’e-mail et de l’audience.
4. Examinez le planning affiché dans la boîte de dialogue. Pour le modifier, utilisez les options de planning décrites dans [Planifier au lancement d’une campagne](/help/coworker/campaigns/schedule-campaign.md), puis enregistrez.
5. Confirmez pour lancer. Une fois l’opération réussie, un message de confirmation s’affiche et le statut de la campagne est mis à jour (défini sur « Planifié » ou « Actif »).

<!-- 
## Input fields / parameters

Not applicable beyond the schedule fields already documented in [Schedule when a campaign launches](/help/coworker/campaigns/schedule-campaign.md) — launching itself doesn't require any additional input. 
-->

## Légendes de l’interface utilisateur

> **Note du rédacteur technique** : des captures d’écran sont nécessaires pour les éléments suivants :

- [ ] Point d’entrée/bouton Launch dans l’en-tête des détails de la campagne
- [ ] Boîte de dialogue de préparation/validation répertoriant les éléments incomplets
- [ ] Boîte de dialogue de lancement affichant l’aperçu e-mail + audience et la section de planning
- [ ] Avis d&#39;impact sur le volume estimé d&#39;envoi (pour les audiences importantes)
- [ ] Message de confirmation de réussite après le lancement
- [ ] Le message « déjà lancé »
- [ ] Message d’erreur générique « launch-failure »

## Ce que cette fonctionnalité ne fait pas

- Elle ne permet pas de lancer une campagne avec un exemple d’audience (non réelle), des e-mails non testés ou des paramètres d’envoi non configurés. Ces trois problèmes doivent d’abord être résolus.
- Le lancement n’accepte pas un planning comme faisant partie de la même action. Le planning est enregistré séparément (à partir de la même boîte de dialogue) avant ou dans le cadre de la confirmation du lancement.
- Il ne prend pas en charge le redémarrage d’une campagne qui a été arrêtée. L’arrêt est <!--(see [Stop a live campaign](./stop-live-campaign.md))-->.
- [ENTRÉES NÉCESSAIRES — à confirmer auprès de l’ingénieur/du chef de projet : pour certains utilisateurs, Launch peut être remplacé par une expérience « à venir » offrant uniquement un téléchargement de campagne (PDF/DOCX) ou un envoi d’e-mail de BAT, sans lancement en libre-service in-app. Confirmez l’audience à laquelle cela s’applique avant de publier, car cela modifie les étapes de procédure pour cette cohorte.]
