---
title: Тип ресурсов планировщика
description: Ресурс **планировщика** — это точка входа для объектной модели Planner. Он возвращает ресурс **планировщика singleton.**  Он не содержит никаких полезных свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8fc5f91dd8da85b259dd792a0926311d57098ee9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470678"
---
# <a name="planner-resource-type"></a>Тип ресурсов планировщика

Пространство имен: microsoft.graph

Ресурс **планировщика** — это точка входа для объектной модели Planner. Он возвращает ресурс **планировщика singleton.**  Он не содержит никаких полезных свойств.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание объекта plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md);| Создайте новый **планировщикBucket,** разместив в коллекции ведер.|
|[Создание объекта plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| Создайте новый **планировщикPlan,** разместив в коллекции планов.|
|[Создание объекта plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md);| Создайте новый **планировщикTask,** разместив в коллекции задач.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|buckets|Коллекция объектов [plannerBucket](plannerbucket.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных ведер|
|планы|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных планов|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных задач|

## <a name="json-representation"></a>Представление JSON
Ниже показано представление ресурса в формате JSON.

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

Ресурс **планировщика** доступен в корне графа.

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
```http
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

