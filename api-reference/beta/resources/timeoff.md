---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 933c940e25c772cede7918dabf62b52ee58f18d2
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657800"
---
# <a name="timeoff-resource-type"></a>Тип ресурса Тимеофф

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Единица измерения, которая не работает в расписании.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание Тимеофф](../api/schedule-post-timesoff.md) | [Тимеофф](timeOff.md) | Создание нового объекта `timeOff`.|
|[Список Тимеоффс](../api/schedule-list-timesoff.md) | Коллекция [тимеофф](timeOff.md) | Получение списка `timeOff` объектов в расписании.|
|[Получение Тимеофф](../api/timeoff-get.md) | [Тимеофф](timeOff.md) | Получение `timeOff` по идентификатору.|
|[Замена Тимеофф](../api/timeoff-put.md) | [Тимеофф](timeOff.md) | Замените элемент `timeOff`.|
|[Удаление Тимеофф](../api/timeoff-delete.md) | Нет | Удаление `timeOff` из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта `timeOff`.|
| userId            |`string`      |Идентификатор пользователя, `timeOff`назначенный. Обязательный.|
| Шаредтимеофф     |`[timeOffItem](timeoffitem.md)`  |Общая версия этого `timeOff` объекта доступна как для сотрудников, так и для руководителей. Обязательный.|
| Драфттимеофф      |`[timeOffItem](timeoffitem.md)`        |Черновая версия этого `timeOff` элемента, просматриваемая руководителями. Обязательный.|
| createdDateTime       |`DateTimeOffset`        |Отметка `timeOff` времени первоначального создания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`        |Отметка `timeOff` времени последнего обновления. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z". |
| lastModifiedBy        |`microsoft.graph.identitySet`        |Удостоверение, которое Последнее обновило `timeOff`. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
