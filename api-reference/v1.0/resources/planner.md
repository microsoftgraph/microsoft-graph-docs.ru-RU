---
title: Тип ресурса планировщика
description: Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f6d25238436b79dec0397df1d005e67e6b17239a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462279"
---
# <a name="planner-resource-type"></a>Тип ресурса планировщика

Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание объекта plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md);| Создание нового **plannerBucket** путем публикации в коллекции "сегменты".|
|[Создание объекта plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| Создание нового **plannerPlan** путем публикации в коллекции plans.|
|[Создание объекта plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md);| Создание нового **plannerTask** путем публикации в коллекции Tasks.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|сегментов|Коллекция [plannerBucket](plannerbucket.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных сегментов|
|планирует|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных планов|
|tasks|Коллекция [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных задач|

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
