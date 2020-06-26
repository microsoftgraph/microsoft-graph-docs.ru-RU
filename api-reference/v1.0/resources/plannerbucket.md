---
title: Тип ресурса plannerBucket
description: ) для задач в плане в Microsoft 365. Он находится в plannerPlan и может иметь коллекцию перечисление plannertasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b424a5ed3aba8bf287ad4d7fe6319504e18b4828
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895568"
---
# <a name="plannerbucket-resource-type"></a>Тип ресурса plannerBucket

Пространство имен: microsoft.graph

Ресурс **plannerBucket** представляет сегмент (или "настраиваемый столбец") для задач в плане в Microsoft 365. Он находится в [plannerPlan](plannerplan.md) и может иметь коллекцию [перечисление plannertasks](plannertask.md).



## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md); |Чтение свойств и связей объекта **plannerBucket** .|
|[Перечисление plannerTasks](../api/plannerbucket-list-tasks.md) |Коллекция [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[Создание](../api/planner-post-buckets.md); | [plannerBucket](plannerbucket.md);   | Создание нового объекта **plannerBucket** . |
|[Update](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md);   |Обновление объекта **plannerBucket** . |
|[Delete](../api/plannerbucket-delete.md) | Нет |Удаление объекта **plannerBucket** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор сегмента. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|name|Строка|Имя сегмента.|
|orderHint|String|Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).|
|planId|Строка|ИДЕНТИФИКАТОР плана, к которому относится сегмент.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Коллекция задач в сегменте.|

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
