---
title: Тип ресурса timeOff
description: Единица, не работая в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9dc8d463e7015ffca2c2b49de503b9a0a3cb5709
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720202"
---
# <a name="timeoff-resource-type"></a>Тип ресурса timeOff

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Единица не работает в расписании.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание](../api/schedule-post-timesoff.md) | [timeOff](timeoff.md) | Создание нового **объекта timeOff.**|
|[List](../api/schedule-list-timesoff.md) | [коллекция timeOff](timeoff.md) | Получите список объектов **timeOff** в этом расписании.|
|[получение](../api/timeoff-get.md); | [timeOff](timeoff.md) | Получите объект **timeOff** по ID.|
|[Replace](../api/timeoff-put.md) | [timeOff](timeoff.md) | Замените **объект timeOff.**|
|[Удаление](../api/timeoff-delete.md) | Нет | Удаление объекта **timeOff** из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта `timeOff`.|
| userId            |`string`      |Идентификатор пользователя, назначенного объекту `timeOff`. Обязательный элемент.|
| sharedTimeOff     | [timeOffItem](timeoffitem.md)  |Общая версия объекта `timeOff`, доступная для просмотра как сотрудникам, так и руководителям. Обязательный элемент.|
| draftTimeOff      | [timeOffItem](timeoffitem.md)        |Черновая версия объекта `timeOff`, доступная для просмотра руководителями. Обязательный элемент.|
| createdDateTime       |`DateTimeOffset`        |Отметка времени, на которой `timeOff` это было впервые создано. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`        |Отпечаток времени, на котором `timeOff` это было в последний раз обновлено. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedBy        | [identitySet](identityset.md)        |Учетная запись, которая последней обновила этот объект `timeOff`. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

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


