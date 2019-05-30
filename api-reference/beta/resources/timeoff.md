---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 060d155b713b46c36dc5c3c4eed433142822857d
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537032"
---
# <a name="timeoff-resource-type"></a>Тип ресурса Тимеофф

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Единица измерения, которая не работает в расписании.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание Тимеофф](../api/schedule-post-timesoff.md) | [Тимеофф](timeoff.md) | Создание нового объекта `timeOff`.|
|[Список Тимеоффс](../api/schedule-list-timesoff.md) | Коллекция [тимеофф](timeoff.md) | Получение списка `timeOff` объектов в расписании.|
|[Получение Тимеофф](../api/timeoff-get.md) | [Тимеофф](timeoff.md) | Получение `timeOff` по идентификатору.|
|[Замена Тимеофф](../api/timeoff-put.md) | [Тимеофф](timeoff.md) | Замена объекта `timeOff`.|
|[Удаление Тимеофф](../api/timeoff-delete.md) | Нет | Удаление `timeOff` из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта `timeOff`.|
| userId            |`string`      |Идентификатор пользователя, `timeOff`назначенный. Обязательно.|
| Шаредтимеофф     | [Тимеоффитем](timeoffitem.md)  |Общая версия этого `timeOff` объекта доступна как для сотрудников, так и для руководителей. Обязательно.|
| Драфттимеофф      | [Тимеоффитем](timeoffitem.md)        |Черновая версия этого `timeOff` элемента, просматриваемая руководителями. Обязательный.|
| createdDateTime       |`DateTimeOffset`        |Отметка `timeOff` времени первоначального создания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`        |Отметка `timeOff` времени последнего обновления. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
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
