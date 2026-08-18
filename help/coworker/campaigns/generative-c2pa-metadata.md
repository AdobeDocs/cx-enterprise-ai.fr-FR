---
description: Découvrez comment les campagnes Coworker joignent et conservent automatiquement les métadonnées C2PA (Content Credentials) sur les images générées et modifiées par l’IA, aucune action n’est requise.
title: Métadonnées C2PA dans les campagnes Coworker
hide: true
source-git-commit: 785b5d106cb029d68506c90385786cbdae164991
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 2%

---

# Métadonnées C2PA dans les campagnes Coworker {#overview}

De nouvelles lois émergent autour de la transparence générative de l’IA, et Adobe s’efforce de répondre aux exigences applicables dans toutes les juridictions. [Métadonnées C2PA](https://c2pa.org/) (également appelées Content Credentials) est l’outil de provenance utilisé par Adobe pour répondre aux exigences de ces lois.

Les métadonnées C2PA sont des métadonnées durables et invisibles qui enregistrent la manière dont un élément de contenu a été créé ou modifié. Lorsque vous générez ou modifiez une image à l’aide d’outils d’IA génératifs dans les campagnes Coworker, des métadonnées C2PA sont automatiquement associées à cette image. Aucune action n’est requise de votre part.

## Actions qui joignent des métadonnées C2PA {#cc-workflows}

Le tableau suivant résume le moment où des métadonnées C2PA sont jointes, en fonction de l’action d’image effectuée dans la génération d’images dans les campagnes Coworker.

| Action | Description | Métadonnées C2PA jointes ? | Exemple de cas d’utilisation |
| --- | --- | --- | --- |
| **Générer une image** | Créez une image à partir d’une invite de texte ou d’une image de référence, ou générez une image similaire à partir d’une image existante. | Toujours. L’image est générée par l’IA générative, elle transfère donc toujours de nouvelles métadonnées C2PA. | Une image de bannière pour une campagne par e-mail est générée à partir d’une invite de texte décrivant le visuel souhaité. |
| **Recadrer une image** (centrer ou recadrer intelligemment) | Ajuster une image aux dimensions demandées | Uniquement si l’image source possédait déjà des métadonnées C2PA. Le recadrage recrée les pixels de l’image, ce qui effacerait normalement ces métadonnées C2PA. De ce fait, la génération d’images dans les campagnes Coworker les lit à partir de l’image source avant de les recadrer, puis les recrée et les relie au résultat recadré. Le recadrage lui-même n&#39;ajoute pas une nouvelle action générative de l&#39;IA : il préserve celle qui existe. | Une image de bannière générée est recadrée pour s’adapter à une page web : les métadonnées C2PA sont conservées par le recadrage. <br> Une photo de catalogue téléchargée utilisée comme arrière-plan de notification push est recadrée pour s’adapter à l’écran : étant donné que la photo de catalogue ne comporte aucune action d’IA générative, aucune métadonnée C2PA n’est créée. |
| **Ajouter une superposition de texte** | Rendu du texte généré sur une image d’arrière-plan | Uniquement si l’image d’arrière-plan contenait déjà des métadonnées C2PA. Le rendu du recouvrement génère une nouvelle image à partir de l’arrière-plan plus le texte, ce qui effacerait normalement ces métadonnées C2PA. De ce fait, la génération d’images dans les campagnes Coworker les lit à l’avance à partir de l’image d’arrière-plan, puis les recrée et les relie au résultat. L’étape de recouvrement n’ajoute pas de nouvelle action d’IA générative. | Un titre promotionnel est rendu sous la forme d’une superposition de texte sur une image d’arrière-plan générée pour une page de destination : les métadonnées C2PA de l’image d’arrière-plan sont conservées. |
| **Recouvrir les images** | Composer deux images ou plus ensemble | Si l’une des images sources comporte des métadonnées C2PA, l’image combinée les transporte toutes, fusionnées en un seul jeu de métadonnées C2PA. La composition produit une nouvelle image à partir des sources, ce qui effacerait normalement ces métadonnées C2PA. De ce fait, la génération d’images dans les campagnes Coworker lit chacune d’elles avant la composition, puis crée un enregistrement de métadonnées C2PA combiné répertoriant chaque source qui a contribué à une action d’IA générative. | Une image de produit générée est composée avec un arrière-plan généré pour un en-tête d’e-mail : le résultat véhicule des métadonnées C2PA reflétant les deux sources d’IA génératives. <br> Deux photos de marque téléchargées sont composites en un seul collage : puisqu’aucune source ne transporte une action d’IA générative, aucune métadonnée C2PA n’est créée. |

## Types de contenu et leur portée {#cc-content-types}

* **Images** : Couvert. Les métadonnées C2PA sont jointes lorsque les images sont générées avec l’IA générative et conservées par le biais d’opérations de recadrage, de superposition de texte et de superposition d’image effectuées par la génération d’images dans les campagnes Coworker.
* **Texte** : sans objet. Les sorties de texte uniquement de la génération d’images dans les campagnes Coworker, telles que la génération de copies, la traduction et les suggestions d’alignement de marque, ne nécessitent pas de métadonnées C2PA.

## Ce qui se passe lorsque le contenu est déplacé {#cc-content-moves}

Les campagnes Coworker conservent le Content Credentials associé aux ressources d’image prises en charge. Si une image contient du Content Credentials lors de son importation dans les campagnes de collègues, ces informations d’identification sont conservées lorsque la ressource est utilisée dans le contenu de campagne généré et les expériences d’e-mail sortant. [En savoir plus sur les métadonnées C2PA](https://helpx.adobe.com/fr/firefly/using/content-credentials.html){target="_blank"}.

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

>[!MORELIKETHIS]
>
>[Instructions d’utilisation de l’IA générative d’Adobe Experience Cloud](https://www.adobe.com/fr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}
