---
title: Тип ресурса planner
description: Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.
ms.openlocfilehash: e5980f6f4037b57e977b12ef223e8a5a2cf7c77c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027717"
---
# <a name="planner-resource-type"></a>Тип ресурса planner

Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание объекта plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| Создайте объект **plannerBucket**, отправив запрос POST в коллекцию buckets.|
|[Создание объекта plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| Создайте объект **plannerPlan**, отправив запрос POST в коллекцию plans.|
|[Создание объекта plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| Создайте объект **plannerTask**, отправив запрос POST в коллекцию tasks.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|buckets|Коллекция объектов [plannerBucket](plannerbucket.md)| Только для чтения. Допускает значение null. Возвращает коллекцию указанных сегментов.|
|plans|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускает значение null. Возвращает коллекцию указанных планов.|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускает значение null. Возвращает коллекцию указанных задач.|

## <a name="json-representation"></a>Представление в формате JSON
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

**Планировщик работы** ресурсов доступна в корне диаграммы.

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