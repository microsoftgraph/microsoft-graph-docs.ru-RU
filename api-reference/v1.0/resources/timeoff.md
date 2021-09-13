---
title: Тип ресурса timeOff
description: Единица, не работая в расписании.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 185f292dbbc8a993699073be1f91b6a2902b18ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59122938"
---
# <a name="timeoff-resource-type"></a>Тип ресурса timeOff

Пространство имен: microsoft.graph

Единица не работает в расписании.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление](../api/schedule-list-timesoff.md) | [коллекция timeOff](timeoff.md) | Получите список объектов **timeOff** в этом расписании.|
|[Создание](../api/schedule-post-timesoff.md) | [timeOff](timeoff.md) | Создание нового **объекта timeOff.**|
|[получение](../api/timeoff-get.md); | [timeOff](timeoff.md) | Получите объект **timeOff** по ID.|
|[Replace](../api/timeoff-put.md) | [timeOff](timeoff.md) | Замените **объект timeOff.**|
|[удаление](../api/timeoff-delete.md); | Нет | Удаление объекта **timeOff** из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |ID **timeOff**.|
| userId            |`string`      |ID пользователя, назначенного **timeOff**. Обязательное.|
| sharedTimeOff     | [timeOffItem](timeoffitem.md)  |Общая версия этого **timeOff,** которая просматривается как сотрудниками, так и руководителями. Обязательный.|
| draftTimeOff      | [timeOffItem](timeoffitem.md)        |Черновик версии этого **timeOff,** который просматривается руководителями. Обязательный.|
| createdDateTime       |`DateTimeOffset`        |Отметка времени, на которой впервые был создан **этот timeOff.** Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`        |Отпечаток времени, на котором в этот **раз был** обновлен последний раз. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedBy        | [identitySet](identityset.md)        |Удостоверение, которое в последний раз обновлялось **в этот раз.** |

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

