---
title: Transparence du contenu d’IA générative
description: Découvrez comment Adobe joint automatiquement les métadonnées C2PA au contenu généré et modifié par GenAI dans les applications d’entreprise Adobe CX.
feature_v2: id: f84b2906-3ce9-4ef0-86f6-cda249273937id: ec4263d9-bf7c-44c7-b3f1-3e664861c8f2
source-git-commit: 4a9ab38cc3aa650dbb90639558d25f6acf707da5
workflow-type: tm+mt
source-wordcount: 1714
ht-degree: 1%

---


# Transparence du contenu d’IA générative

Tout au long du mois d’août 2026, Adobe déploie progressivement la prise en charge des métadonnées C2PA sur les applications Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly et Adobe CX Enterprise.

>[!NOTE]
>
>Suite au déploiement, les futurs workflows dont le contenu est créé ou modifié à l’aide de l’IA disposeront automatiquement de la prise en charge des métadonnées C2PA.

Cette page présente en détail la façon dont Adobe gère la pièce jointe automatique des métadonnées C2PA dans les applications Adobe CX Enterprise.

Les nouvelles réglementations exigent des fournisseurs de technologies d’IA génératives qu’ils prennent en charge les divulgations durables et lisibles par machine associées aux workflows de contenu générés et modifiés par GenAI, pour plus de transparence.

En tant que fournisseur d’outils, Adobe joint automatiquement des métadonnées C2PA lisibles par machine au contenu généré et modifié par GenAI à l’aide des technologies Adobe (y compris les modèles d’IA générés tiers pris en charge dans les workflows Adobe). [En savoir plus sur C2PA](https://c2pa.org/).

## Changements en cours

Déployé en août 2026, Adobe introduira la prise en charge des métadonnées C2PA dans les applications Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly et Adobe CX Enterprise.

Cette version comprend les éléments suivants :

* La pièce jointe automatique des métadonnées C2PA au contenu généré et modifié par GenAI pris en charge.
* Prise en charge des types de contenu, notamment les images, les vidéos, l’audio et le texte.
* Conservation des métadonnées C2PA dans tous les workflows Adobe pris en charge.

Aucune action supplémentaire n’est requise pour joindre des métadonnées C2PA au contenu d’IA génératif éligible.

>[!NOTE]
>
>Les métadonnées C2PA n’auront aucune incidence sur l’aspect de votre contenu. Les métadonnées C2PA et les filigranes visibles ont des objectifs différents. Les métadonnées C2PA fournissent des informations de provenance lisibles par machine, tandis que les filigranes visibles fournissent une divulgation visuelle. Vous pouvez choisir d’ajouter des filigranes visibles à votre contenu en fonction des besoins de l’entreprise et des exigences légales de chaque juridiction applicable.

## Détails ajoutés dans le cadre des métadonnées C2PA

Les métadonnées C2PA automatiquement associées peuvent inclure des informations telles que :

* Nom et informations de version du système d’IA utilisé (par exemple, Adobe GenStudio ou Adobe Firefly)
* Modèle d’IA utilisé (par exemple, Adobe Firefly)
* Utilisation : s’il a été généré ou modifié à l’aide de GenAI
* Date et heure de création et/ou de modification du contenu avec les outils d’IA génératifs
* Identifiant unique (qui peut être utilisé pour distinguer chaque utilisation de l’IA générative)

## Métadonnées C2PA dans le supply chain de contenu

Les métadonnées C2PA sont conçues pour rester associées au contenu pris en charge lorsqu’il passe d’une application Adobe à une plateforme tierce compatible.

Lorsque le contenu est publié, distribué ou partagé, les plateformes qui prennent en charge les métadonnées C2PA ou les technologies de provenance associées peuvent lire les métadonnées jointes et afficher des informations de transparence aux utilisateurs.

Adobe ne contrôle pas la manière dont les services externes interprètent, affichent ou utilisent les métadonnées C2PA après que le contenu a quitté les applications Adobe. Les clients doivent consulter la documentation relative aux plateformes de publication individuelles pour comprendre comment les métadonnées C2PA sont gérées.

## Filigrane visible

Dans certaines circonstances et dans certaines zones géographiques, les organisations peuvent choisir ou être tenues d’identifier de manière visible le contenu généré ou modifié par GenAI.

Adobe fournit des [conseils](https://helpx.adobe.com/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html) sur l’utilisation des fonctionnalités d’application de filigrane existantes prises en charge par les applications Adobe. L’utilisation d’un filigrane visible dépend des exigences commerciales d’une organisation et des lois et réglementations en vigueur dans les juridictions où le contenu est publié.

>[!NOTE]
>
>Les métadonnées C2PA et les filigranes visibles ont des objectifs différents. Les métadonnées C2PA fournissent des informations de provenance lisibles par machine, tandis que les filigranes visibles fournissent une divulgation visuelle que les organisations peuvent choisir d’appliquer.

## Disponibilité et versions

Ces fonctionnalités sont déployées tout au long de **août 2026** dans les workflows Adobe CX Enterprise pris en charge.

>[!NOTE]
>
>Suite au déploiement, les futurs workflows dont le contenu est créé ou modifié à l’aide de l’IA disposeront automatiquement de la prise en charge des métadonnées C2PA.

Cette version comprend les éléments suivants :

### Métadonnées C2PA automatiques

Les métadonnées C2PA sont automatiquement associées au contenu généré et modifié par GenAI pris en charge. Cette fonctionnalité est activée par défaut et ne peut pas être désactivée.

### Conseils sur les filigranes

Adobe fournit [documentation](https://helpx.adobe.com/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html) décrivant comment utiliser les fonctionnalités d’application d’un filigrane disponibles dans les applications Adobe prises en charge pour les organisations qui choisissent ou doivent appliquer des libellés visibles.

## Applications prises en charge dans Adobe CX Enterprise {#supported-applications}

Les applications et services Adobe ci-après fournissent des informations supplémentaires sur la manière et le moment où les métadonnées C2PA sont jointes au contenu éligible dans certaines applications d’entreprise CX.

Cependant, le cas échéant, toutes les applications d’entreprise Adobe CX continuent à conserver les métadonnées C2PA existantes au fur et à mesure que les ressources prises en charge passent par les workflows Adobe. Cela permet de préserver l’intégrité des informations de provenance dans l’ensemble du supply chain de contenu.

>[!NOTE]
>
>Les notes de mise à jour ou conseils relatifs à chacune des applications répertoriées ci-dessous seront disponibles sur Experience League dans les sections respectives de leur page produit d’application. Le tableau sera mis à jour avec les liens dès qu’ils seront disponibles. Reportez-vous aux dernières sections produit sur Experience League.

| Application/Solution | Notes de mise à jour/conseils |
|---|---|
| Adobe Advertising Cloud | [Documentation](https://experienceleague.adobe.com/en/docs/advertising/creative/creative-studio/creative-studio-content-credentials) |
| Adobe Experience Manager (AEM) | [Documentation](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/c2pa-metadata-dynamic-media-openapi) |
| Assistant AI pour la génération de contenu (fonctionnalité dans Adobe Journey Optimizer/Adobe Campaign) | [Documentation](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/generate-content/generative-c2pa-metadata) |
| Adobe Journey Optimizer B2B Ultimate | [Documentation](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/content-management/assets/c2pa-metadata) |
| Prime B2B Adobe Journey Optimizer (ou Adobe Marketo Optimizer) | [Documentation](https://experienceleague.adobe.com/en/docs/marketo-optimizer/user/content/assets/c2pa-metadata) |
| Adobe Journey Optimizer B2C | |
| Adobe Campaign | |
| Adobe Commerce | [Documentation](https://experienceleague.adobe.com/en/docs/commerce/optimizer/manage-results/success-metrics#c2pa-metadata-on-exported-reports) |
| GenStudio for Performance Marketing | [Documentation](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/content-credentials) |
| Adobe Marketo Engage | [Documentation](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/c2pa-metadata) |
| Adobe Workfront | [Documentation](https://experienceleague.adobe.com/en/docs/workfront/using/documents/c2pa-metadata-overview) |
| Campagnes des collaborateurs des entreprises CX (anciennement HALO) | [Documentation](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/c2pa-metadata) |

## Liens connexes

* [Guide des filigranes visibles](https://helpx.adobe.com/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)
* [Adobe Inspect](https://contentauthenticity.adobe.com/inspect)
* [Présentation de l’initiative de conformité à l’étiquetage GenAI d’Adobe](https://helpx.adobe.com/creative-cloud/apps/generative-ai/ai-content-labeling-faq.html)

## Questions fréquentes

**Quelles applications Adobe appliquent des métadonnées C2PA au contenu généré modifié ou créé par l’IA ?**

Les applications Adobe CX Enterprise prises en charge joignent automatiquement des métadonnées C2PA au contenu généré et modifié par GenAI éligible. Reportez-vous à la section [Applications prises en charge](#supported-applications) pour plus d’informations sur les applications Adobe CX Enterprise.

**À quels types de contenu Adobe ajoute-t-il des métadonnées C2PA ?**

En règle générale, les images, l’audio, la vidéo, les documents et le texte sont concernés. Toutefois, reportez-vous à la documentation de la section [Applications prises en charge](#supported-applications) pour savoir comment chaque application prend en charge les métadonnées C2PA pour différents produits et types de contenu.

**Quelles sont les applications d’Adobe CX qui conservent les métadonnées C2PA tout au long de la modification et de la publication ?**

Toutes les applications Adobe CX Enterprise sont conçues pour conserver les métadonnées C2PA pendant le déplacement du contenu dans les workflows Adobe compatibles. La conservation en dehors des applications Adobe dépend de la prise en charge ou non des métadonnées C2PA par les plateformes externes.

**Que se passe-t-il lorsque plusieurs images générées par GenAI sont combinées en une seule image ?**

Les métadonnées C2PA qui en résultent dépendent de l’application et du workflow utilisés. Lorsqu’il est pris en charge, Adobe conserve les informations de provenance tout au long du processus de modification. Reportez-vous à la section [Applications prises en charge](#supported-applications-across-adobe-cx-enterprise) de la documentation pour connaître le comportement spécifique aux workflows dans chaque application.

**Que se passe-t-il lorsque des images générées par GenAI à partir d’applications Adobe et non Adobe sont combinées ?**

Adobe conserve les métadonnées C2PA qui sont disponibles et prises en charge dans le workflow. Le cas échéant, Adobe met à jour les métadonnées sous-jacentes avec les dernières informations chaque fois que le contenu applicable (image, audio, vidéo, texte) est modifié ou créé à l’aide de GenAI dans les workflows Adobe. Lorsque vous combinez plusieurs sources en une seule nouvelle ressource, leurs métadonnées sous-jacentes ne sont ni remplacées ni perdues. Au lieu de cela, la nouvelle ressource obtient ses propres métadonnées C2PA, et les détails de chaque source sont conservés à l’intérieur de celle-ci. Si une source possédait déjà ses propres métadonnées C2PA, qu’elles proviennent d’un outil Adobe ou d’un outil autre qu’Adobe, cet historique reste associé. Cela signifie que la ressource finale présente une image complète : son propre enregistrement de création ou d’édition avec GenAI, ainsi que l’historique individuel de chaque élément qui y a été intégré.

**Les workflows modifiés par GenAI et créés par GenAI dans les applications Adobe CX joignent-ils automatiquement des métadonnées C2PA ?**

Oui. Pour les workflows d’IA générative pris en charge, Adobe joint automatiquement des métadonnées C2PA qui identifient si le contenu a été généré par GenAI ou modifié par GenAI, ainsi que d’autres informations de provenance, telles que des horodatages, des informations système d’IA et des identifiants uniques.

**Comment les métadonnées C2PA sont-elles conservées dans l’ensemble de la supply chain de contenu ?**

Les métadonnées C2PA sont des métadonnées durables conçues pour rester associées au contenu pris en charge lors de son déplacement entre les applications Adobe compatibles et les plateformes tierces de prise en charge. Les services externes déterminent comment les informations de provenance jointes s’affichent après publication.

**Comment les organisations peuvent-elles ajouter leurs propres informations authentifiées sans rompre la chaîne de provenance ?**

Certaines applications Adobe permettent aux créateurs et aux organisations d’ajouter des informations authentifiées supplémentaires aux métadonnées C2PA existantes tout en préservant la provenance. La disponibilité varie selon l’application.

**Est-il possible de désactiver la connexion automatique des métadonnées C2PA ?**

Non. Les nouvelles lois sur la transparence de l’IA générative exigent des entreprises qui fournissent des outils d’IA générative, notamment Adobe, qu’elles joignent des métadonnées durables au contenu éligible généré ou modifié avec l’IA générative. Impossible de désactiver la pièce jointe automatique des métadonnées C2PA.

**Qu’advient-il du contenu créé/modifié avec l’IA générative avant la publication d’août ?**

Le contenu créé ou modifié avec des outils d’IA génératifs avant la version d’août 2026 n’est pas associé à des métadonnées C2PA automatiques. Cependant, le contenu créé dans Firefly Web et d’autres applications où les métadonnées C2PA étaient précédemment appliquées continue à être joint.

**Comment un client peut-il vérifier si des métadonnées C2PA sont associées au contenu ?**

Les clients peuvent vérifier si des métadonnées C2PA sont associées au contenu en le chargeant sur la page [Adobe Inspect](https://contentauthenticity.adobe.com/inspect).

**Comment les plateformes externes affichent-elles les métadonnées C2PA une fois le contenu publié ou partagé ?**

À mesure que le contenu se déplace sur les plateformes de publication, les canaux de médias sociaux, les services de messagerie électronique et d’autres écosystèmes numériques, les services en aval qui prennent en charge les métadonnées C2PA ou les technologies de provenance associées peuvent être en mesure de lire les métadonnées jointes et de choisir d’afficher les divulgations ou les indicateurs en fonction de ces informations. Adobe ne contrôle pas la manière dont les plateformes externes affichent, interprètent ou appliquent les divulgations associées aux métadonnées C2PA jointes. Pour obtenir les informations les plus récentes sur la façon dont une plateforme spécifique gère les informations de provenance, les clients doivent vérifier directement les directives de cette plateforme.

**Ces modifications augmentent-elles le coût des produits ou des abonnements Adobe ?**

Non. Les métadonnées C2PA n’ont aucune incidence sur le coût des produits Adobe.
