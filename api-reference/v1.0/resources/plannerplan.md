---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Microsoft 365. План может принадлежать группе. Он содержит коллекцию объектов plannerTask. Кроме того, он может содержать коллекцию объектов plannerBucket. Каждому объекту plan соответствует объект details, который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье "Планировщик".
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b5b27469f08caf764031030a88c35d2f976a5dd3f420cdf6221ab858f2ccd137
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243322"
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
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания плана. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String| Только для чтения. Идентификатор плана. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|owner|String|Идентификатор [группы](group.md), которая является владельцем плана. Чтобы в этом поле можно было указать значение, должна существовать подходящая группа. После установки значения обновить это свойство невозможно.|
|title|String|Обязательный. Название плана.|
|createdBy|[identitySet](identityset.md)|Только для чтения. Пользователь, создавший этот план.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|buckets|Коллекция объектов [plannerBucket](plannerbucket.md)| Только для чтения. Допускает значение null. Коллекция контейнеров в плане.|
|details|[plannerPlanDetails](plannerplandetails.md)| Только для чтения. Допускает значение null. Дополнительные сведения о плане.|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускает значение null. Коллекция задач в плане.|

## <a name="json-representation"></a>Представление в формате JSON

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
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
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

