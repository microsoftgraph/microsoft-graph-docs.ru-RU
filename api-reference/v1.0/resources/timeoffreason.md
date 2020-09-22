---
title: Тип ресурса Тимеоффреасон
description: Представляет допустимую причину для выполнения времени ожидания в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 1630cf2c76ca98f8637af9c80900daf97bcc5660
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090790"
---
# <a name="timeoffreason-resource-type"></a>Тип ресурса Тимеоффреасон

Пространство имен: microsoft.graph

Представляет допустимую причину для экземпляра [тимеофф](timeoff.md) по [расписанию](schedule.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление](../api/schedule-list-timeoffreasons.md) | Коллекция [тимеоффреасон](timeoffreason.md) | Получение списка **тимеоффреасон** по расписанию.|
|[Создание](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | Создание нового **тимеоффреасон**.|
|[Получение](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | Получение **тимеоффреасон** по идентификатору.|
|[Replace](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | Замените **тимеоффреасон**.|
|[удаление](../api/timeoffreason-delete.md); | Нет | Пометка **тимеоффреасон** как неактивной.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта `timeOffReason`.|
| displayName               | `string`                  | Имя **тимеоффреасон**. Обязательный. |
| иконтипе | `timeOffReasonIconType`   | Поддерживаемые типы значков: нет; Мойка ведения запускается ходил Фирстаид; врача Нотворкинг; регистрации Журидути; любой кружк звонков Погода Общий Пиггибанк; Dog очень Траффикконе; крепления Веселая. Обязательный. |
| isActive          |`Boolean`      | Указывает, можно ли использовать **тимеоффреасон** при создании новых сущностей или обновлении существующих. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Отметка времени первоначального создания **тимеоффреасон** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`         |Отметка времени последнего обновления **тимеоффреасон** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedBy        | [identitySet](identityset.md)        |Удостоверение, которое последним обновило этот **тимеоффреасон**.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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

