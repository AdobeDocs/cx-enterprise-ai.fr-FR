---
title: Outils Adobe Experience Platform dans la passerelle CX Coworker
description: Découvrez les outils Adobe Experience Platform disponibles via la passerelle CX Coworker.
source-git-commit: 30f4d593bdec8cb45d10c4c49fac3dce16e8ca03
workflow-type: tm+mt
source-wordcount: '1372'
ht-degree: 8%

---


# Outils Adobe Experience Platform dans la passerelle Adobe CX Coworker {#aep-mcp}

Vous pouvez utiliser les outils du produit Adobe Experience Platform pour inspecter les schémas, les jeux de données, la configuration de la gouvernance des données, les ressources de Query Service et les événements d’audit d’un client compatible avec MCP. Ces outils sont disponibles via la passerelle Adobe CX Coworker [](overview.md) lorsque votre organisation est activée et que votre compte utilisateur dispose des autorisations Experience Platform requises.

>[!AVAILABILITY]
>
>L’outil de produit Experience Platform se trouve dans Beta. L’accès se fait sur invitation uniquement et nécessite l’activation de l’organisation Adobe. Voir [Accéder aux outils de passerelle de collègue CX](access.md).

## Résumé

| Outil | Description | Ressource | Fonctionnalités | Statut |
| --- | --- | --- | --- | --- |
| `search_allowed_ip_ranges` | Récupération des restrictions d’accès IP de Query Service | Authentification Data Distiller · Plages d’adresses IP | list | Actif |
| `search_audit` | Répertorier les événements d’audit d’activité des utilisateurs dans Experience Platform | Requête d’audit · événements d’audit | liste, filtrage par type de ressource, action, statut, période | Actif |
| `search_datasets` | Requête sur les métadonnées d’ingestion par lots et de jeu de données | API de catalogue · jeux de données, lots | list, get, filter, list last, list files | Actif |
| `search_class_relations` | Rechercher dans les relations de classe affaires d’Experience Platform | Relations de classe · index YAML statique | recherche par jeton, terme multiple, correspondance partielle | Actif |
| `search_data_access` | Répertorier les fichiers des lots d’ingestion ayant échoué | API Data Access · lots ayant échoué | répertorier les fichiers ayant échoué | Actif |
| `search_data_lake` | Inspecter les métadonnées du jeu de données et l’intégrité des lots | API du lac de données · jeux de données, lots | obtenir, obtenir la taille, répertorier les lots ayant échoué | Actif |
| `search_dule` | Étiquettes, politiques et actions de gouvernance des données de requête | Gouvernance des données · libellés, politiques, actions marketing | list, get, list enabled, evaluation | Actif |
| `search_query_service` | Requête Requêtes SQL, modèles, plannings, alertes | Query Service · requêtes, modèles, plannings, alertes | liste, get, filter, get paramètres de connexion | Actif |
| `search_schema_registry` | Schémas XDM de requête, groupes de champs, classes, types | Registre des schémas · schémas, groupes de champs, classes, data_types, descripteurs | lister, obtenir, filtrer par conteneur | Actif |

## Référence de l&#39;outil

### search_allowed_ip_range

**Ressource :** Authentification Data Distiller · Plages d’adresses IP
**Statut:** Actif

Récupérez toutes les restrictions d’accès IP configurées pour Query Service dans le sandbox actuel. Renvoie l’identifiant de l’organisation et la liste des plages d’adresses IP autorisées. Disponible uniquement pour les clients et clientes qui utilisent le module complémentaire Distiller de données.

**Fonctionnalités :** répertorie les plages d’adresses IP autorisées pour Query Service.

Aucun paramètre.

### search_audit

**Ressource :** Requête d’audit · événements d’audit
**Statut:** Actif

Répertorier les enregistrements horodatés des activités utilisateur dans les services Experience Platform. Renvoie le type d’action, l’e-mail de l’utilisateur, les informations sur la ressource et le statut de l’événement. Utilisez `asset_type` et `action` pour limiter les résultats. La valeur par défaut est les 7 derniers jours lorsqu’aucune période n’est spécifiée. Limité aux 1 000 derniers enregistrements et événements des 90 derniers jours.

**Fonctionnalités :** répertorier les événements d’audit, filtrer par type de ressource, action, statut, période, paginer

**Paramètres:**

| Paramètre | Obligatoire | Description |
| --- | --- | --- |
| `action` | Non | Filtrez par type d’action. Valeurs courantes (séparées par des virgules pour OR) : `Create`, `Delete`, `Update`, `Enable`, `Disable` |
| `asset_type` | Non | Filtrez par type de ressource. Doit être l’un des éléments suivants : `Dataset`, `Schema`, `Segment`, `Destination`, `Source Data Flow`, `Merge Policy`, `Identity Namespace`, `Identity Graph`, `Sandbox`, `Role`, `Query`, `Scheduled Query`, `Datastream`, `Computed Attribute`, `Field Group`, `Class`, `Data Types`, `Account`, `Product Profile`, `Query Template`, `Work Order`, `Audit Logs`, `Access Control Policy`,,, |
| `status` | Non | Filtrez par statut d’événement. Valeurs : `Success`, `Failure`, `Allow`, `Deny`. Séparé par une virgule pour OU |
| `start_time` | Non | Date et heure au plus tôt. ISO 8601 UTC avec ms, par exemple `2024-01-15T00:00:00.000Z` |
| `end_time` | Non | Dernière date et heure. ISO 8601 UTC avec ms |
| `property_filter` | Non | Expression de filtre brute, par exemple `action==create`. Préférez les paramètres dédiés ci-dessus |
| `orderby` | Non | Ordre de tri : `timestamp` (asc) ou `-timestamp` (desc) |
| `limit` | Non | Nombre maximal de résultats (3-1 000, 50 par défaut) |
| `start` | Non | Décalage de pagination. Incrémenter par valeur limite pour chaque page |
| `query_id` | Non | Identifiant de requête d’une réponse précédente pour répéter la même requête |

### search_datasets

**Ressource :** API de catalogue · jeux de données, lots
**Statut:** Actif

Outil de répartition unifié pour le service de catalogue Experience Platform. Requête sur les enregistrements de jeu de données (références de schéma, balises, informations de création) ou d’ingestion par lots (statut, mesures, listes de fichiers). Utilisez `dataset/list` pour découvrir les jeux de données, `batch/list` pour vérifier l’intégrité de l’ingestion et `batch/list_files` ou `batch/get_meta_files` pour inspecter le contenu de lots spécifiques. Toutes les opérations sont en lecture seule.

**Fonctionnalités :** répertorier les jeux de données, obtenir le jeu de données, répertorier les lots, obtenir le lot, répertorier le dernier lot par jeu de données, répertorier les fichiers de lot, obtenir les métafichiers de lot (erreurs de ligne, fichiers d’entrée)

**Paramètres:**

| Paramètre | Obligatoire | Description |
| --- | --- | --- |
| `entity_type` | Oui | `dataset` ou `batch`. |
| `operation` | Oui | `list`, `get`, `list_last`, `list_files`, `get_meta_files`. Combinaisons valides : liste des → de jeux de données, get ; lot → les cinq |
| `resource_id` | Non | Jeu de données ou ID de lot. Requis pour `dataset/get`, `batch/get`, `batch/list_files`, `batch/get_meta_files` |
| `query_params.limit` | Non | Résultats max. par page (100 max.). S’applique à toutes les opérations de liste |
| `query_params.start` | Non | Décalage de pagination. S’applique à toutes les opérations de liste |
| `query_params.order_by` | Non | Direction de tri, par exemple `asc:created,updated`. S’applique à toutes les opérations de liste |
| `query_params.properties` | Non | Propriété séparée par des virgules. S’applique à dataset/list, dataset/get, batch/list, batch/list_last |
| `query_params.name` | Non | Filtrer les jeux de données par nom (jeu de données/liste uniquement) |
| `query_params.tags` | Non | Filtrage des jeux de données par balises, par exemple `unifiedProfile:enabled:true` (jeu de données/liste uniquement) |
| `query_params.property_filter` | Non | Filtre Regex sur les objets de réponse (jeu de données/liste et lot/liste) |
| `query_params.status` | Non | Filtrer les lots par statut : `success`, `failed`, `loading`, `active` (lot/liste uniquement) |
| `query_params.dataset_id` | Non | Étendue des lots à un jeu de données spécifique (batch/list et batch/list_last) |
| `query_params.created_after` | Non | Filtrer les lots créés après l’horodatage Unix en ms (lot/liste uniquement) |
| `query_params.created_before` | Non | Filtrer les lots créés avant l’horodatage Unix en ms (lot/liste uniquement) |
| `query_params.last_batch_status` | Non | Filtrer par statut du dernier lot (batch/list_last only) |
| `query_params.aggregate` | Non | Renvoi de mesures agrégées au niveau racine (batch/get uniquement) |
| `query_params.path` | Non | Fichier Meta à télécharger : `row_errors`, `input_files`, `row_errors_sample.json` (batch/get_meta_files uniquement) |

### search_class_relations

**Ressource :** Relations de classe · index YAML statique
**Statut:** Actif

Recherchez des relations de classe commerciale Experience Platform par nom à l’aide de l’index de `class_relations_v1.yaml` statique. Aucun appel d’API Experience Platform n’est effectué. Accepte un seul terme ou des termes séparés par des virgules ; chaque terme est mis en correspondance avec des noms de classe à l’aide d’une correspondance de jeton partielle. Renvoie les classes correspondantes avec des relations directes (ce vers quoi chaque classe pointe) et des relations inverses (quelles classes lui renvoient). Utilisez ceci pour comprendre les relations d’entité avant de créer des requêtes, des flux de données ou des compositions de schéma.

**Fonctionnalités :** recherche par jeton, recherche multi-terme séparée par des virgules, correspondance de jeton partielle, extension de synonyme bidirectionnelle

**Paramètres:**

| Paramètre | Obligatoire | Description |
| --- | --- | --- |
| `query` | Oui | Nom de la classe professionnelle ou type d’objet à rechercher. Prend en charge les correspondances de jeton partielles (`dat` correspond à `dataset`, `data_type`, etc.). Transmettez plusieurs termes séparés par des virgules pour rechercher plusieurs classes à la fois (par exemple, `dataset, schema`) |
| `n` | Non | Nombre maximal de résultats correspondants à renvoyer (5 par défaut, min 1) |

### search_data_access

**Ressource :** API Data Access · lots ayant échoué
**Statut:** Actif

Accédez aux fichiers des lots d’ingestion de données Experience Platform ayant échoué. Utilisez `failed_batch/list_failed` pour répertorier les fichiers appartenant à un lot en échec pour le diagnostic des échecs. Nécessite un identifiant de lot pour toutes les opérations. Remarque : `file/get` et `dataset/preview` sont désactivés car ils exposent les données d’enregistrement réelles. Toutes les opérations sont en lecture seule.

**Fonctionnalités :** répertorie les fichiers d’un lot d’ingestion en échec

**Paramètres:**

| Paramètre | Obligatoire | Description |
| --- | --- | --- |
| `entity_type` | Oui | `failed_batch` — répertorie les fichiers d&#39;un lot d&#39;ingestion ayant échoué |
| `operation` | Oui | `list_failed` : la seule opération prise en charge |
| `resource_id` | Oui | Identifiant du lot en échec |
| `query_params.start` | Non | Index de début de la pagination, par exemple `1` |
| `query_params.limit` | Non | Nombre de résultats par page, par exemple `10` |
| `query_params.path` | Non | Filtre de nom de fichier complet ; `profiles.csv`, par exemple |


### search_data_lake

**Ressource :** API du lac de données · jeux de données, lots
**Statut:** Actif

Inspectez les métadonnées du jeu de données et du lot à partir de la couche du lac de données. Utilisez `get` pour les métadonnées complètes, `get_size` pour les mesures de taille de stockage et d’ingestion, et `list_failed` pour surveiller les échecs d’ingestion dans une fenêtre temporelle. La valeur par défaut est les 7 derniers jours lorsqu’aucune période n’est fournie pour `list_failed`. Toutes les opérations sont en lecture seule et nécessitent un identifiant de ressource.

**Fonctionnalités :** obtenir des métadonnées de jeu de données/lot, obtenir des mesures de taille de stockage, répertorier les lots en échec dans une fenêtre temporelle

**Paramètres:**

| Paramètre | Obligatoire | Description |
| --- | --- | --- |
| `entity_type` | Oui | `dataset` ou `batch`. |
| `operation` | Oui | `get`, `get_size`, `list_failed`. `list_failed` ne prend en charge que le type d’entité `batch` |
| `resource_id` | Oui | Identifiant du jeu de données ou de lot. Par `list_failed` : identifiant du jeu de données pour définir l’étendue des échecs sur |
| `query_params.created_after` | Non | Début de la fenêtre temporelle. Date et heure Unix en ms |
| `query_params.created_before` | Non | Fin de la fenêtre temporelle. Date et heure Unix en ms |
| `query_params.limit` | Non | Résultats max. par page (100 max.) |
| `query_params.order_by` | Non | Direction de tri, par exemple `desc:created` |

### search_dule

**Ressource :** Gouvernance des données · libellés, politiques, actions marketing
**Statut:** Actif

Recherchez des libellés d’utilisation des données, des politiques et des actions marketing dans l’API Policy Service. Utilisez `marketing_action/evaluate` pour tester si une action marketing sur des données avec des libellés spécifiques enfreindrait les politiques de gouvernance. Toutes les opérations sont en lecture seule.

**Fonctionnalités :** lister/obtenir des libellés d’utilisation des données, lister/obtenir des politiques, lister les politiques activées, lister/obtenir des actions marketing, évaluer l’action marketing par rapport aux libellés

**Paramètres:**

| Paramètre | Obligatoire | Description |
| --- | --- | --- |
| `entity_type` | Oui | `label`, `policy` ou `marketing_action` |
| `operation` | Oui | `list`, `get`, `list_enabled` (politique uniquement), `evaluate` (marketing_action uniquement). `list_enabled` ne nécessite pas de portée |
| `scope` | Non | `core` (défini par Adobe) ou `custom` (défini par l’organisation). Requis pour `list`, `get`, `evaluate` ; non utilisé pour `list_enabled` |
| `resource_id` | Non | Nom du libellé, ID de la politique ou nom de l’action marketing. Requis pour `get` et `evaluate` |
| `query_params.dule_labels` | Non | Libellés séparés par des virgules (par exemple, `C1,C3`). Obligatoire pour `marketing_action/evaluate` ; filtre facultatif pour `policy/list` |
| `query_params.limit` | Non | Résultats max |
| `query_params.start` | Non | Curseur de pagination à partir de la valeur de `_page.next` d’une réponse précédente |
| `query_params.orderby` | Non | Champs de tri séparés par des virgules |
| `query_params.property_filter` | Non | Expression de filtre, par exemple `name==C1` |
| `query_params.marketing_action` | Non | Restreindre la liste des politiques aux politiques qui font référence à cette action marketing (politique/liste uniquement) |
| `query_params.include_draft` | Non | Inclure les BROUILLONS de politiques dans `marketing_action/evaluate` (par défaut : POLITIQUES ACTIVÉES uniquement) |

### search_query_service

**Ressource :** Query Service · requêtes, modèles, plannings, exécutions de planning, connexions, abonnements aux alertes
**Statut:** Actif

Outil unifié pour les ressources de Query Service. Répertoriez et récupérez les requêtes ad hoc, les modèles SQL enregistrés, les requêtes planifiées et leurs exécutions, les paramètres de connexion interactive (pour les clients psql/JDBC) et les abonnements aux alertes. Pour les listes de requêtes, utilisez par défaut `isService==false,isParentLevel==true` pour filtrer le trafic interne. Toutes les opérations sont en lecture seule.

**Fonctionnalités :** des requêtes list/get, modèles list/get, list/get plannings, exécutions list/get schedule, get connection params, list alert subscriptions

**Paramètres:**

| Paramètre | Obligatoire | Description |
| --- | --- | --- |
| `entity_type` | Oui | `query`, `query_template`, `schedule`, `schedule_run`, `connection`, `alert_subscription` |
| `operation` | Oui | `list`, `get`, `get_connection_params`, `list_by_u...` |
