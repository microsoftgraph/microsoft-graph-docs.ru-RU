---
title: Тип ресурса plannerUser
description: 'Ресурс **plannerUser** предоставляет доступ к ресурсам, планировщик работы для пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1b240092e7476884399f88fad61551763f33fe69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928285"
---
# <a name="planneruser-resource-type"></a>Тип ресурса plannerUser

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerUser** предоставляет доступ к ресурсам планировщик работы для [пользователей](user.md). 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление задач](../api/planneruser-list-tasks.md) |Коллекция объектов [plannerTask](plannertask.md)| Получите [plannerTasks](plannertask.md) , назначенные пользователю.|
|[Список favoritePlans](../api/planneruser-list-favoriteplans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получите [plannerPlans](plannerplan.md) , помеченные как избранные пользователем.|
|[Список recentPlans](../api/planneruser-list-recentplans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получите [plannerPlans](plannerplan.md) недавно отображаемое для пользователя.|
|[обновление](../api/planneruser-update.md). | [plannerUser](planneruser.md)| Обновление объекта **plannerUser** . |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор plannerUser|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md);| Коллекция, содержащая ссылки на планы, которые пользователь помеченные как "Избранное".|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md).| Коллекция, содержащая ссылки на планы, которые были просмотрены недавно пользователя в приложениях, которые поддерживают последние планов.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускает значение null. Возвращает объекты [plannerTask](plannertask.md), назначенные пользователю.|
|favoritePlans|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает [plannerPlans](plannerplan.md) , пользователь помеченные как "Избранное".|
|recentPlans|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает [plannerPlans](plannerplan.md) , который был недавно доступен для просмотра пользователем в приложениях, которые поддерживают последние планов. |

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
