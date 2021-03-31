---
title: тип ресурса accessReviewQueryScope
description: Определяет, что будет рассмотрено в обзоре доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 976a856755b6bb638719bec6006c3d8d0587c42a
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469798"
---
# <a name="accessreviewqueryscope-resource-type"></a>тип ресурса accessReviewQueryScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Объект accessReviewQueryScope определяет, что будет рассмотрено в [accessReview.](../resources/accessreviewsv2-root.md) В поддерживаемых запросах см. параметры выбора. Чтобы просмотреть обзор доступа для неактивных пользователей, см. [в примере accessReviewInactiveUserQueryScope.](../resources/accessreviewinactiveusersqueryscope.md) 

Наследует [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Запрос|String|Запрос, представляющий то, что будет рассмотрено в обзоре доступа. Примеры этого включают /groups/{id}/members?$filter=...|
|queryRoot|String|В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса. Это свойство необходимо только в том случае, если указан относительный запрос. Например, `./manager`.|
|queryType|String|Указывает тип запроса. Типы включают MicrosoftGraph и ARM.|

### <a name="supported-queries-for-accessreviewqueryscope-as-scope"></a>Поддерживаемые запросы для accessReviewQueryScope в качестве области
Запросы поддерживаются как `scope` свойство [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Сценарий| Запрос | Дополнительные комментарии |
|--|--|-- |
| Просмотр всех пользователей, назначенных группе | /groups/{group id}/transitiveMembers ||
| Просмотр гостевых пользователей, назначенных группе | /groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest') ||
| Обзор гостевых пользователей, присвоенных всем группам Microsoft 365 | ./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest') | Обратите внимание, что соответствующий экземплярEnumerationScope также следует передать в accessReviewScheduleDefinition. См. таблицу ниже, например запросEnumerationScope. |
| Отзывы о назначении пакета назначения пакета управления правами | /identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')| Обратите внимание, что только READ поддерживается для отзывов о назначении пакета доступа|
| Обзор директоров служб, назначенных привилегированным ролям | /beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}') | |

### <a name="supported-queries-for-instanceenumerationscope"></a>Поддерживаемые запросы, напримерEnumerationScope 
Запросы поддерживаются как `instanceEnumerationScope` свойство [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Сценарий| Запрос | Дополнительные комментарии |
|--|--|--|
|  Обзор гостевых пользователей, присвоенных всем группам Microsoft 365| /v1.0/groups? \$ filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true | Обратите внимание, что соответствующая область также должна быть передана вместе с этим|
| Просмотр гостевых пользователей, назначенных всем группам | /v1.0/groups? \$ filter=(groupTypes/any(c:c+eq+'Unified) и resourceProvisioningOptions/Any (x:x eq 'Team'))&$count=true | Обратите внимание, что соответствующая область также должна быть передана вместе с этим|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
