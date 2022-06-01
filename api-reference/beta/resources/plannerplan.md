---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Microsoft 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждый объект плана имеет объект сведений, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8972c3073cb11a7c008a52503b4a4b4a8c231487
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821283"
---
# <a name="plannerplan-resource-type"></a>Тип ресурса plannerPlan

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerPlan** представляет план в Microsoft 365. План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md). Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md). Каждый объект плана имеет объект [сведений](plannerplandetails.md) , который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).



## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |Считывание свойств и связей объекта **plannerPlan**.|
|[Перечисление контейнеров](../api/plannerplan-list-buckets.md) |Коллекция [plannerBucket](plannerbucket.md)| Получение коллекции объектов **plannerBucket**.|
|[Перечисление задач](../api/plannerplan-list-tasks.md) |Коллекция объектов [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[Обновление](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |Обновление объекта **plannerPlan**. |
|[Удаление](../api/plannerplan-delete.md) | Нет | Удаление **объекта plannerPlan** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|контейнер|[plannerPlanContainer](../resources/plannerplancontainer.md)|Определяет контейнер плана. После установки значения обновить это свойство невозможно. Обязательный.|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания плана. Тип "Метка времени" представляет информацию о дате и времени в формате ISO 8601 и всегда соответствует времени в стандарте UTC. Например, полночь в стандарте UTC 1 января 2014 года равна`2014-01-01T00:00:00Z`|
|id|String| Только для чтения. Идентификатор плана. Содержит 28 знаков, учитывается регистр. [Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.|
|title|String|Обязательный. Название плана.|
|createdBy|[identitySet](identityset.md)|Только для чтения. Пользователь, создавший этот план.|
|Контекстах|[plannerPlanContextCollection](plannerplancontextcollection.md);| Только для чтения. Дополнительные пользовательские возможности, в которых используется этот план, представлены в виде [записей plannerPlanContext](plannerplancontext.md) .|
|владелец (не рекомендуется) |String| Вместо этого используйте свойство **контейнера**. Идентификатор [группы](group.md), которая является владельцем плана. После установки значения обновить это свойство невозможно. Это свойство не возвращает допустимый идентификатор группы, если контейнер плана не является группой.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|buckets|Коллекция объектов [plannerBucket](plannerbucket.md)| Коллекция контейнеров в плане. Только для чтения. Допускается значение null.|
|details|[plannerPlanDetails](plannerplandetails.md)| Дополнительные сведения о плане. Только для чтения. Допускается значение null. |
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Коллекция задач в плане. Только для чтения. Допускается значение null. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "url": "String",
    "containerId": "String",
    "type": "String"
  },
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


