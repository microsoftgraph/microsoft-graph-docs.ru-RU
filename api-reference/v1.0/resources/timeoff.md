---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 1c33ed74b52983b9adc3ce0d1c729caaa35dce09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090832"
---
# <a name="timeoff-resource-type"></a>Тип ресурса Тимеофф

Пространство имен: microsoft.graph

Единица измерения "не работает" в расписании.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление](../api/schedule-list-timesoff.md) | Коллекция [тимеофф](timeoff.md) | Получение списка объектов **тимеофф** в этом расписании.|
|[Создание](../api/schedule-post-timesoff.md) | [timeOff](timeoff.md) | Создание нового объекта **тимеофф** .|
|[Получение](../api/timeoff-get.md) | [timeOff](timeoff.md) | Получение объекта **тимеофф** по идентификатору.|
|[Replace](../api/timeoff-put.md) | [timeOff](timeoff.md) | Замена объекта **тимеофф** .|
|[удаление](../api/timeoff-delete.md); | Нет | Удаление объекта **тимеофф** из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта **тимеофф**.|
| userId            |`string`      |Идентификатор пользователя, назначенный **тимеофф**. Обязательный.|
| шаредтимеофф     | [тимеоффитем](timeoffitem.md)  |Общая версия этого **тимеофф** , которая доступна для сотрудников и руководителей. Обязательный.|
| драфттимеофф      | [тимеоффитем](timeoffitem.md)        |Черновая версия этого **тимеофф** , которая отображается руководителями. Обязательный.|
| createdDateTime       |`DateTimeOffset`        |Отметка времени первоначального создания **тимеофф** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`        |Отметка времени последнего обновления **тимеофф** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedBy        | [identitySet](identityset.md)        |Удостоверение, которое последним обновило этот **тимеофф**. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"},
  "draftTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"}
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
  "suppressions": []
}
-->

