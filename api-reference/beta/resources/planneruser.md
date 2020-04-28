---
title: Тип ресурса plannerUser
description: 'Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 70ca7596cfb809a16b76f684a85c97b0c3e43a50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521638"
---
# <a name="planneruser-resource-type"></a>Тип ресурса plannerUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для [пользователя](user.md). 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление задач](../api/planneruser-list-tasks.md) |Коллекция [plannerTask](plannertask.md)| Получение [перечисление plannertasks](plannertask.md) , назначенных пользователю.|
|[Список объектов favoritePlans](../api/planneruser-list-favoriteplans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получите [планов](plannerplan.md) , помеченный пользователем как избранный.|
|[Список объектов recentPlans](../api/planneruser-list-recentplans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получение [планов](plannerplan.md) , недавно просмотренных пользователем.|
|[обновление](../api/planneruser-update.md). | [plannerUser](planneruser.md)| Обновление объекта **plannerUser** . |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор объекта plannerUser|
|фаворитепланреференцес|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md);| Коллекция, содержащая ссылки на планы, помеченные пользователем как "Избранное".|
|рецентпланреференцес|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md).| Коллекция, содержащая ссылки на планы, которые пользователь недавно просматривал в приложениях, поддерживающих последние планы.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Возвращает [перечисление plannertasks](plannertask.md) , назначенный пользователю.|
|фаворитепланс|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает [планов](plannerplan.md) , отмеченный пользователем как "Избранное".|
|рецентпланс|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает [планов](plannerplan.md) , которые недавно просматривал пользователь в приложениях, которые поддерживают последние планы. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "suppressions": []
}
-->
