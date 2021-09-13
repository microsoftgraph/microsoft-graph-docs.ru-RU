---
title: тип ресурса plannerBucket
description: ) для задач в плане в Microsoft 365. Он содержится в планировщикеPlan и может иметь коллекцию plannerTasks.
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 46360d413f676e6420f28b94b5ba91ec9237e681
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129848"
---
# <a name="plannerbucket-resource-type"></a>тип ресурса plannerBucket

Пространство имен: microsoft.graph

Ресурс **plannerBucket** представляет ведро (или "настраиваемый столбец") для задач в плане в Microsoft 365. Он содержится в [планировщикеPlan](plannerplan.md) и может иметь коллекцию [plannerTasks.](plannertask.md)



## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |Чтение свойств и связей **объекта plannerBucket.**|
|[Перечисление plannerTasks](../api/plannerbucket-list-tasks.md) |Коллекция [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[Создание](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | Создание нового **объекта plannerBucket.** |
|[Обновление](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |Объект **Update plannerBucket.** |
|[удаление](../api/plannerbucket-delete.md); | Нет |Удаление **объекта plannerBucket.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. ID из ведра. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|name|String|Имя сегмента.|
|orderHint|String|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).|
|planId|Строка|Запланируйте ID, к которому принадлежит ведро.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Коллекция задач в ведре.|

## <a name="json-representation"></a>Представление JSON
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

