---
title: Тип ресурса reminder
description: Напоминание о событии в календаре пользователя.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cc07c6e8b787925e9ee72dbb949997c18ca70f87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446991"
---
# <a name="reminder-resource-type"></a>Тип ресурса reminder

Пространство имен: microsoft.graph

Напоминание о [событии](event.md) в [календаре](calendar.md)пользователя.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|changeKey|String|Указывает версию напоминания. При каждом изменении напоминания также меняется значение **changeKey**. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|евентендтиме|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс завершения события.|
|Диапазоне|String|Уникальный идентификатор события. Только для чтения.|
|евентлокатион|[Location](location.md)|Место проведения события.|
|евентстарттиме|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс начала события.|
|евентсубжект|String|Текст в строке темы сообщения о событии.|
|евентвеблинк|String|URL-адрес для открытия события в Outlook в Интернете.<br/><br/>Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br/><br/>Доступ к этому URL-адресу можно получить из объекта iFrame.|
|реминдерфиретиме|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, заданные для упоминания.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
