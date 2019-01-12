---
title: Тип ресурса plannerBucket
description: ) для выполнения задач в плане в Office 365. Она содержится в plannerPlan и можно создать свою коллекцию plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 8cfc25e5554b20d4f808c8929b53549f4c44d7a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982836"
---
# <a name="plannerbucket-resource-type"></a>Тип ресурса plannerBucket

Ресурс **plannerBucket** представляет сегмент (или "специальный столбец") для задач плана в Office 365. Он содержится в объекте [plannerPlan](plannerplan.md) и может содержать коллекцию объектов [plannerTasks](plannertask.md).



## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |Чтение свойств и отношений объекта **plannerBucket**.|
|[Перечисление объектов plannerTasks](../api/plannerbucket-list-tasks.md) |Коллекция объектов [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[Создание](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | Создание объекта **plannerBucket**. |
|[Обновление](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |Обновление объекта **plannerBucket**. |
|[Удаление](../api/plannerbucket-delete.md) | Нет |Удаление объекта **plannerBucket**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка| Только для чтения. Идентификатор сегмента. Это 28 знаков без учета регистра. [Формат](planner-identifiers-disclaimer.md) проверяются на службу.|
|name|Строка|Имя сегмента.|
|orderHint|Строка|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).|
|planId|Строка|Идентификатор плана, к которому относится сегмент.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускает значение null. Коллекция задач в сегменте.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
