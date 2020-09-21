---
title: Тип ресурса планировщика
description: Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8333596ee93a42db8eded49815059e8633bf3db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037635"
---
# <a name="planner-resource-type"></a>Тип ресурса планировщика

Пространство имен: microsoft.graph

Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание объекта plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md);| Создание нового **plannerBucket** путем публикации в коллекции "сегменты".|
|[Создание объекта plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| Создание нового **plannerPlan** путем публикации в коллекции plans.|
|[Создание объекта plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md);| Создание нового **plannerTask** путем публикации в коллекции Tasks.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|buckets|Коллекция объектов [plannerBucket](plannerbucket.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных сегментов|
|планирует|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных планов|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных задач|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a>Пример

Ресурс **планировщика** доступен в корневом каталоге диаграммы.

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

