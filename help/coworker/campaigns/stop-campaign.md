---
description: La description est ici.
title: Arrêter une campagne
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 410
ht-degree: 1%

---

# Arrêter une campagne {#stop-campaign}

Les utilisateurs peuvent désormais arrêter une campagne qui envoie activement (une campagne « active ») directement à partir de la page des détails de la campagne. L’arrêt d’une campagne est permanent : les destinataires arrêtent immédiatement de progresser dans la campagne et la campagne ne peut pas reprendre ni redémarrer par la suite.

## Conditions préalables

- La campagne doit être active (envoi actif). L’action Arrêter n’est pas disponible pour les campagnes en version brouillon, planifiées ou déjà arrêtées.
- [ENTRÉES NÉCESSAIRES — à confirmer auprès de l’ingénieur : l’arrêt d’une campagne nécessite-t-il un rôle ou une autorisation spécifique, ou un utilisateur disposant d’un accès à la campagne peut-il le faire ?]

## Fonctionnement de cette fonctionnalité

Une action « Arrêter la campagne » s’affiche dans l’en-tête des détails de la campagne chaque fois qu’une campagne est active. Si vous la sélectionnez, une boîte de dialogue de confirmation s’affiche pour vous informer que l’action est permanente. La confirmation appelle le serveur principal pour arrêter la campagne ; en cas de réussite, le statut de la campagne devient « Arrêté » et un message de confirmation s’affiche.

### Comportements clés

- L’action Arrêter la campagne ne s’affiche que lorsqu’une campagne est active (envoi actif).
- L’arrêt est permanent : les destinataires arrêtent de progresser dans la campagne et celle-ci ne peut pas reprendre.
- Une boîte de dialogue de confirmation nécessite que l’utilisateur confirme explicitement avant l’arrêt de la campagne.
- Après l’arrêt, le badge d’état de la campagne est mis à jour sur « Arrêté ».
- Si la demande d’arrêt échoue, un message d’erreur s’affiche et la campagne reste active.

## Comment l’utiliser

1. Ouvrez une campagne actuellement active (envoi actif).
2. Dans l’en-tête des détails de la campagne, cliquez sur **Arrêter la campagne**.
3. Dans la boîte de dialogue de confirmation, passez en revue l’avertissement : « L’arrêt de la campagne est permanent. Tous les destinataires cesseront de progresser et la campagne ne pourra pas reprendre. »
4. Cliquez sur **Arrêter** pour confirmer.
5. Une « campagne arrêtée ». Un message de confirmation apparaît et le statut de la campagne est mis à jour sur « Arrêté ».

### Champs/paramètres de saisie

Sans objet : cette fonctionnalité est une action de confirmation unique sans champs d’entrée.

## Légendes de l’interface utilisateur

> **Note du rédacteur technique** : des captures d’écran sont nécessaires pour les éléments suivants :

- [ ] Le bouton « Arrêter la campagne » dans l’en-tête des détails de la campagne, affiché sur une campagne active
- [ ] Boîte de dialogue de confirmation contenant l’avertissement de permanence
- [ ] Le badge d’état « Arrêté » après un arrêt réussi
- [ ] Message d’erreur affiché en cas d’échec de l’arrêt

## Ce que cette fonctionnalité ne fait pas

- Il ne met pas temporairement une campagne en pause. Il n’existe aucun moyen de reprendre une campagne arrêtée ; l’arrêt est une action à sens unique.
- Il ne prend pas en charge le redémarrage ou la relance d’une campagne arrêtée à partir du même enregistrement de campagne.
- [ENTRÉES NÉCESSAIRES — à confirmer auprès de l’ingénieur : une fonctionnalité « pause et reprise » distincte est-elle prévue, ou l’option Arrêter est-elle la seule action de contrôle d’état fournie dans cette version ?]
