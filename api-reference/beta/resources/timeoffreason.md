---
title: Тип ресурса Тимеоффреасон
description: Допустимая причина для выполнения времени ожидания в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3a08ad02b03b3b39385f6f351e727d8b5ed54af1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075485"
---
# <a name="timeoffreason-resource-type"></a>Тип ресурса Тимеоффреасон

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Допустимая причина для экземпляра [тимеофф](timeoff.md) по [расписанию](schedule.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | Создание нового **тимеоффреасон**.|
|[Список](../api/schedule-list-timeoffreasons.md) | Коллекция [тимеоффреасон](timeoffreason.md) | Получение списка **тимеоффреасон** по расписанию.|
|[получение](../api/timeoffreason-get.md); | [timeOffReason](timeoffreason.md) | Получение **тимеоффреасон** по идентификатору.|
|[Replace](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | Замените **тимеоффреасон**.|
|[Удаление](../api/timeoffreason-delete.md) | Нет | Пометка **тимеоффреасон** как неактивной.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта `timeOffReason`.|
| displayName               | `string`                  | Имя ресурса `timeOffReason`. Обязательно. |
| иконтипе | `timeOffReasonIconType`   | Поддерживаемые типы значков: нет; Мойка ведения запускается ходил Фирстаид; врача Нотворкинг; регистрации Журидути; любой кружк звонков Погода Общий Пиггибанк; Dog очень Траффикконе; крепления Веселая. Обязательный. |
| isActive          |`Boolean`      | Указывает, можно ли использовать объект `timeOffReason` при создании новых сущностей или обновлении существующих. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Отметка времени `timeOffReason` первоначального создания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`         |Отметка времени `timeOffReason` последнего обновления. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedBy        | [identitySet](identityset.md)        |Учетная запись, которая последней обновила этот объект `timeOffReason`.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "iconType": "String",
  "isActive": true,
  "lastModifiedBy": { "@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


