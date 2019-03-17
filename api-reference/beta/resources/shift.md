---
title: Тип ресурса Shift
description: Смена — это единица запланированной работы в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c392bfb4a1691ab99d852febdda27cdf1c3b8044
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657898"
---
# <a name="shift-resource-type"></a>Тип ресурса Shift

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Единица запланированной работы по [расписанию](schedule.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание смены](../api/schedule-post-shifts.md) | [перемещен](shift.md) | Создание нового `shift`объекта.|
|[ПереЧисление смещений](../api/schedule-list-shifts.md) | Коллекция " [SHIFT](shift.md) " | Получение списка `shifts` по данному расписанию.|
|[Получение Shift](../api/shift-get.md) | [перемещен](shift.md) | Получение `shift` по идентификатору.|
|[Замена Shift](../api/shift-put.md) | [перемещен](shift.md) | Замените элемент `shift`.|
|[Удаление смены](../api/shift-delete.md) | Нет | Удаление `shift` из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта `shift`.|
| userId            |`string`      |Идентификатор пользователя, `shift`назначенный. Обязательный. |
| Счедулингграупид         |`string`      |Идентификатор группы планирования, в которой `shift` входит. Обязательный. |
| Шаредшифт   |`[shiftItem](shiftitem.md)`  |Общая версия этого `shift` объекта доступна как для сотрудников, так и для руководителей. Обязательный. |
| Драфтшифт        |`[shiftItem](shiftitem.md)`        |Черновая версия этого `shift` элемента, просматриваемая руководителями. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Временная метка, на которую `shift` был создан впервые. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`        |Отметка времени `shift` последнего обновления. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z". |
| lastModifiedBy        |`microsoft.graph.identitySet`        |Удостоверение, которое Последнее обновило `shift`.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shift.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
