---
title: Тип ресурса plannerBucket
description: ) для задач в плане в Microsoft 365. Он находится в plannerPlan и может иметь коллекцию перечисление plannertasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 02c8ef4dc25d43ee1fdd57a939bd0ed69ba86b81
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073607"
---
# <a name="plannerbucket-resource-type"></a>Тип ресурса plannerBucket

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerBucket** представляет сегмент (или "настраиваемый столбец") для задач в плане в Microsoft 365. Он находится в [plannerPlan](plannerplan.md) и может иметь коллекцию [перечисление plannertasks](plannertask.md).



## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md); |Чтение свойств и связей объекта **plannerBucket** .|
|[Перечисление plannerTasks](../api/plannerbucket-list-tasks.md) |Коллекция [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[Создание](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md);   | Создание нового объекта **plannerBucket** . |
|[Обновление](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md);   |Обновление объекта **plannerBucket** . |
|[Удаление](../api/plannerbucket-delete.md) | Нет |Удаление объекта **plannerBucket** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор сегмента. Содержит 28 знаков, учитывается регистр. [Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.|
|name|String|Имя сегмента.|
|orderHint|String|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).|
|planId|Строка|ИДЕНТИФИКАТОР плана, к которому относится сегмент.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Коллекция задач в сегменте.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


