---
title: Тип ресурса plannerBucket
description: Представляет контейнер для задач в плане в Microsoft 365. Он содержится в планировщике и может содержать коллекцию plannerTasks.
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a13e219c4d31fc129e7f5561e61a073d635d41c1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212646"
---
# <a name="plannerbucket-resource-type"></a>Тип ресурса plannerBucket

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контейнер (или "настраиваемый столбец") для задач в плане в Microsoft 365. Он содержится в [планировщике и](plannerplan.md) может содержать коллекцию [plannerTasks](plannertask.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md); |Чтение свойств и связей объекта **plannerBucket** .|
|[Перечисление plannerTasks](../api/plannerbucket-list-tasks.md) |Коллекция [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[Создание](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md);   | Создайте объект **plannerBucket** . |
|[Обновление](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md);   |Обновление **объекта plannerBucket** . |
|[удаление](../api/plannerbucket-delete.md); | Нет |Удаление **объекта plannerBucket** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор контейнера. Содержит 28 знаков, учитывается регистр. [Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.|
|name|String|Имя сегмента.|
|orderHint|String|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).|
|planId|Строка|Идентификатор плана, к которому принадлежит контейнер.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Коллекция задач в контейнере.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.

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


