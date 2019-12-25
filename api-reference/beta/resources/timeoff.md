---
title: Тип ресурса Тимеофф
description: Единица измерения, которая не работает в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 64ef8a07d3190ad2a54e9e3e5c68f3ffb0335acc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866527"
---
# <a name="timeoff-resource-type"></a>Тип ресурса Тимеофф

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Единица измерения "не работает" в расписании.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание](../api/schedule-post-timesoff.md) | [тимеофф](timeoff.md) | Создание нового объекта **тимеофф** .|
|[List](../api/schedule-list-timesoff.md) | Коллекция [тимеофф](timeoff.md) | Получение списка объектов **тимеофф** в этом расписании.|
|[Get (.. /АПИ/тимеофф-жет.МД) | [тимеофф](timeoff.md) | Получение объекта **тимеофф** по идентификатору.|
|[Replace](../api/timeoff-put.md) | [тимеофф](timeoff.md) | Замена объекта **тимеофф** .|
|[удаление](../api/timeoff-delete.md); | Нет. | Удаление объекта **тимеофф** из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта `timeOff`.|
| userId            |`string`      |Идентификатор пользователя, назначенного объекту `timeOff`. Обязательный атрибут.|
| шаредтимеофф     | [тимеоффитем](timeoffitem.md)  |Общая версия объекта `timeOff`, доступная для просмотра как сотрудникам, так и руководителям. Обязательный атрибут.|
| драфттимеофф      | [тимеоффитем](timeoffitem.md)        |Черновая версия объекта `timeOff`, доступная для просмотра руководителями. Обязательный элемент.|
| createdDateTime       |`DateTimeOffset`        |Отметка `timeOff` времени первоначального создания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`        |Отметка `timeOff` времени последнего обновления. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
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
