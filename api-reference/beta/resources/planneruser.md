---
title: Тип ресурса plannerUser
description: 'Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563673"
---
# <a name="planneruser-resource-type"></a>Тип ресурса plannerUser

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для [пользователя](user.md). 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление задач](../api/planneruser-list-tasks.md) |Коллекция [plannerTask](plannertask.md)| Получение [перечисление plannertasks](plannertask.md) , назначенных пользователю.|
|[Список Фаворитепланс](../api/planneruser-list-favoriteplans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получите [планов](plannerplan.md) , помеченный пользователем как избранный.|
|[Список Рецентпланс](../api/planneruser-list-recentplans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получение [планов](plannerplan.md) , недавно просмотренных пользователем.|
|[Обновление](../api/planneruser-update.md) | [plannerUser](planneruser.md)| Обновление объекта **plannerUser** . |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор объекта plannerUser|
|Фаворитепланреференцес|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md);| Коллекция, содержащая ссылки на планы, помеченные пользователем как "Избранное".|
|Рецентпланреференцес|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md).| Коллекция, содержащая ссылки на планы, которые пользователь недавно просматривал в приложениях, поддерживающих последние планы.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|tasks|Коллекция [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Возвращает [перечисление plannertasks](plannertask.md) , назначенный пользователю.|
|Фаворитепланс|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает [планов](plannerplan.md) , отмеченный пользователем как "Избранное".|
|Рецентпланс|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает [планов](plannerplan.md) , которые недавно просматривал пользователь в приложениях, которые поддерживают последние планы. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planneruser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
