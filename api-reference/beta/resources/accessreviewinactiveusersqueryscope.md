---
title: accessReviewInactiveUsersQueryScope
description: Тип accessReviewQueryScope, который позволяет выбирать только неактивных пользователей в области обзора доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 51fc61ce186b0346bc065ddc5dfea40158758223
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469799"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>accessReviewInactiveUsersQueryScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Тип [accessReviewQueryScope,](../resources/accessreviewqueryscope.md) который позволяет выбирать только неактивных пользователей в области обзора доступа.

Наследует [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|inactiveDuration|Duration|Определяет продолжительность периода бездействия. Неактивность основана на последнем знаке даты пользователя.|
|Запрос|String|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryRoot|String|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryType|String|Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).|

### <a name="supported-queries-for-accessreviewinactiveuserqueryscope-as-scope"></a>Поддерживаемые запросы для accessReviewInactiveUserQueryScope в качестве области
Те же запросы, поддерживаемые [в accessReviewScope,](../resources/accessreviewscope.md) также поддерживаются в accessReviewInactiveUserQueryScope. Ниже приводится запрос. Они поддерживаются как `scope` свойство [в accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)

|Сценарий| Запрос |
|--|--|
| Просмотр всех неактивных гостевых пользователей, назначенных группе | /groups/{group ID}/transitiveMembers/microsoft.graph.user/? \$ count=true&$filter=(userType eq 'Guest') |
| Просмотр всех неактивных пользователей, заметив группу | /groups/{group ID}/transitiveMembers |
| Просмотр всех неактивных гостевых пользователей, назначенных всем группам | ./members/microsoft.graph.user/? \$ count=true&$filter=(userType eq 'Guest') |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
