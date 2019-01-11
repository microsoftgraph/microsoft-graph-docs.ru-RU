---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе и содержит коллекцию plannerTasks. Он также может иметь коллекцию plannerBuckets. Каждый объект плана имеет объект сведений, который может содержать дополнительные сведения о плане. Дополнительные сведения о связях между группами, планы и задачи можно планировщик работы.
localization_priority: Priority
ms.openlocfilehash: cfcc94fab067cc76bb530edbdb8477183ebf3531
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873012"
---
# <a name="plannerplan-resource-type"></a>Тип ресурса plannerPlan

Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannertask.md). Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerbucket.md). Каждый объект plan имеет объект [details](plannerplandetails.md), который может содержать дополнительные сведения о плане. Дополнительные сведения об отношениях, которыми связаны группы, планы и задачи, см. в статье [Планировщик](planner-overview.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |Считывание свойств и связей объекта **plannerPlan**.|
|[Перечисление сегментов](../api/plannerplan-list-buckets.md) |Коллекция объектов [plannerBucket](plannerbucket.md)| Получение коллекции объектов **plannerBucket**.|
|[Перечисление задач](../api/plannerplan-list-tasks.md) |Коллекция объектов [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[обновление](../api/plannerplan-update.md). | [plannerPlan](plannerplan.md) |Обновление объекта **plannerPlan**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания плана. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|Строка| Только для чтения. Идентификатор плана. Это 28 знаков без учета регистра. [Формат](planner-identifiers-disclaimer.md) проверяются на службу.|
|owner|Строка|Идентификатор [группы](group.md) , который несет ответственность за планирование. В этом поле можно указать допустимое группы должен существовать. После его установки, это свойство не удается обновить.|
|title|String|Обязательный. Название плана.|
|createdBy|[identitySet](identityset.md)|Только для чтения. Пользователь, создавший этот план.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|buckets|Коллекция объектов [plannerBucket](plannerbucket.md)| Только для чтения. Допускает значение null. Коллекция контейнеров в плане.|
|details|[plannerPlanDetails](plannerplandetails.md);| Только для чтения. Допускает значение null. Дополнительные сведения о плане.|
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
