---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Microsoft 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждому объекту plan соответствует объект details, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
ms.localizationpriority: high
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 53497ac4745cecc18d86fe3341da43118ea22210
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420602"
---
# <a name="plannerplan-resource-type"></a>Тип ресурса plannerPlan

Пространство имен: microsoft.graph

Ресурс **plannerPlan** представляет план в Microsoft 365. План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md). Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md). Каждому объекту plan соответствует объект [details](plannerplandetails.md), который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |Считывание свойств и связей объекта **plannerPlan**.|
|[Перечисление контейнеров](../api/plannerplan-list-buckets.md) |Коллекция [plannerBucket](plannerbucket.md)| Получение коллекции объектов **plannerBucket**.|
|[Перечисление задач](../api/plannerplan-list-tasks.md) |Коллекция объектов [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[Обновление](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |Обновление объекта **plannerPlan**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|контейнер|[plannerPlanContainer](../resources/plannerplancontainer.md)|Определяет контейнер плана. После установки значения обновить это свойство невозможно. Обязательно.|
|createdBy|[identitySet](identityset.md)|Только для чтения. Пользователь, создавший этот план.|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания плана. Тип "Метка времени" представляет информацию о дате и времени в формате ISO 8601 и всегда соответствует времени в стандарте UTC. Например, полночь в стандарте UTC 1 января 2014 года равна`2014-01-01T00:00:00Z`|
|id|String| Только для чтения. Идентификатор плана. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|title|String|Обязательный. Название плана.|
|владелец (не рекомендуется) |String| Вместо этого используйте свойство **контейнера**. Идентификатор [группы](group.md), которая является владельцем плана. После установки значения обновить это свойство невозможно. Это свойство не возвращает допустимый идентификатор группы, если контейнер плана не является группой.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|buckets|Коллекция объектов [plannerBucket](plannerbucket.md)| Только для чтения. Допускает значение null. Коллекция контейнеров в плане.|
|details|[plannerPlanDetails](plannerplandetails.md)| Только для чтения. Допускает значение null. Дополнительные сведения о плане.|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускает значение null. Коллекция задач в плане.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "containerId": "String",
    "type": "String",
    "url": "String"
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

