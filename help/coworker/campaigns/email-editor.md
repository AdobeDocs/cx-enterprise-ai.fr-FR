---
description: description.
title: Comprendre l’éditeur d’e-mail
source-git-commit: e5992ce91452c98e043e8367d7cc551d6914647b
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Comprendre l’éditeur d’e-mail {#email-editor}

L’éditeur d’email permet d’affiner un email généré par l’IA directement sur le tableau de campagne. Modifiez l’objet et le pré-titre, mettez en forme le texte et les images sur la ligne ou remplacez-les dans un autre modèle. <!-- It's an inline editor over the email's actual HTML, not a drag-and-drop block builder. -->

>[!PREREQUISITES]
>
>Créez une campagne avec un email généré.

## Fonctionnement de cette fonctionnalité

Cliquez sur une carte d’e-mail dans le tableau de bord de la campagne pour ouvrir l’éditeur d’e-mail sous forme de panneau latéral. À partir de là, l’utilisateur peut modifier l’objet et le pré-titre (avec des alternatives suggérées par l’IA), cliquer dans le corps de l’e-mail pour sélectionner et formater le texte ou les images, basculer entre des variantes générées par l’IA, échanger le modèle HTML, vérifier la compatibilité client-e-mail et envoyer un e-mail de test dans sa propre boîte de réception. Les modifications sont enregistrées automatiquement et les versions antérieures peuvent être examinées et restaurées.

### Comportements clés

- Cliquez sur n’importe quel texte ou image du corps de l’e-mail pour le sélectionner et afficher une barre d’outils de mise en forme flottante.
- Options de mise en forme de texte : gras, italique, souligné, police et taille de police.
- Options d’image : Remplacer, Supprimer, Lier, Modifier avec Express, Générer une image (IA), Télécharger depuis un ordinateur.
- Les chargements d’images sont limités à 10 Mo ; les images de plus de 3 Mo sont automatiquement compressées, avec une note de qualité recommandant les images de moins de 3 Mo.
- Les champs d’objet et de pré-titre comportent chacun une option « Suggestions intelligentes » pour les alternatives générées par l’IA.
- Modifications enregistrées automatiquement (sur flou et peu de temps après les actions de formatage) : un indicateur de statut indique Modifications non enregistrées, Enregistrement en cours..., Enregistré, Enregistré automatiquement ou Impossible d’enregistrer (avec une option Réessayer ).
- L’option Annuler/rétablir est disponible pour la session de modification actuelle.
- Les versions enregistrées précédentes peuvent être prévisualisées et restaurées à partir d’un panneau d’historique des versions.
- S’il existe plusieurs variantes générées par l’IA, l’utilisateur peut basculer entre elles à partir d’un panneau de miniatures.
- Le modèle HTML de l’e-mail peut être remplacé à l’aide de « Changer de modèle HTML ».
- L’option « Envoyer un e-mail de test » envoie un aperçu réel dans la boîte de réception de l’utilisateur à l’aide de données d’exemple ; elle n’affecte pas les rapports de campagne.
- Une vérification de la compatibilité client-e-mail est disponible dans certains environnements, notamment Gmail, Outlook, Apple Mail, Yahoo Mail, Samsung Email et Thunderbird. [ENTRÉES NÉCESSAIRES — Ceci se trouve derrière un indicateur de fonctionnalité ; vérifiez s&#39;il est activé pour le public cible avant de le documenter comme étant généralement disponible]

## Accès

1. Ouvrez la campagne souhaitée et cliquez sur Ouvrir l’éditeur dans la carte d’e-mail.

CAPTURE D’ÉCRAN

1. Modifiez directement les champs **Objet** et **Pré-titre** ou cliquez sur **Suggestions intelligentes** en regard de pour accéder à des alternatives générées par l’IA.
1. Cliquez dans le corps de l’e-mail pour sélectionner un bloc de texte ou une image, puis utilisez la barre d’outils flottante qui s’affiche pour mettre en forme le texte ou gérer l’image.
1. Utilisez **Changer de modèle HTML** pour remplacer le corps de l’e-mail par un modèle différent.
1. Utilisez **Envoyer un e-mail de test**, saisissez l’adresse d’un destinataire et cliquez sur **Envoyer** pour envoyer un aperçu dynamique par e-mail à cette adresse.
1. Utilisez l’icône d’historique de versions pour prévisualiser et restaurer une version enregistrée antérieure.
1. Les modifications sont enregistrées automatiquement : aucune étape d’enregistrement manuel n’est requise.

### Champs/paramètres de saisie

| Champ | Description | Obligatoire ? |
| --- | --- | --- |
| Objet | Objet de l’e-mail | Non (peut être laissé vide ; actuellement non appliqué) |
| Pré-titre | Texte d’aperçu affiché en regard de l’objet dans une boîte de réception | Non |
| Adresse e-mail du destinataire | Où envoyer un email de test | Oui, pour Envoyer un e-mail de test |

## Légendes de l’interface utilisateur

> **Note du rédacteur technique** : des captures d’écran sont nécessaires pour les éléments suivants :

- [ ] Panneau latéral de l’éditeur d’e-mail (champs objet/pré-titre et corps de l’e-mail)
- [ ] Barre d’outils flottante pour la sélection de texte
- [ ] La barre d’outils flottante pour la sélection d’images
- [ ] le panneau des miniatures des variantes de l’IA
- [ ] Le panneau Historique des versions
- [ ] la boîte de dialogue « Changer de modèle HTML »
- [ ] Boîte de dialogue Envoyer un e-mail de test
- [ ] Vérificateur de compatibilité client-e-mail (s’il est activé dans l’environnement cible)

## Ce que cette fonctionnalité ne fait pas

- Il ne s’agit pas d’un créateur de blocs par glisser-déposer : il n’y a pas de bibliothèque de blocs et les blocs de contenu ne peuvent pas être ajoutés, supprimés ou réorganisés ; la modification se fait directement sur l’email HTML existant.
- Actuellement, il ne prend pas en charge l’insertion de balises de personnalisation/fusion.
- Il ne fournit pas de champ de texte secondaire pour les images.
- Il n’impose pas de vérification de l’objet, du pré-titre ni d’autres vérifications au niveau du contenu avant qu’un e-mail ne soit considéré comme « prêt » ; les seules vérifications avant le lancement sont au niveau de la campagne (configuration de l’envoi, e-mail de test envoyé, audience réelle), et non pas des vérifications sur le contenu de l’e-mail lui-même.
- Le basculement de l’aperçu pour ordinateur/mobile n’est pas disponible dans la vue d’édition d’e-mail de Campaign standard. [ENTRÉES NÉCESSAIRES pour confirmer la portée]
- [ENTRÉES NÉCESSAIRES — à confirmer auprès de l’ingénieur : si l’éditeur devient entièrement en lecture seule (et pas seulement le champ expéditeur) une fois qu’une campagne a été activée/lancée.]
