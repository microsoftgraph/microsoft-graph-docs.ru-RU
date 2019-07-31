---
title: Тип ресурса reminder
description: Напоминание о событии в календаре пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4b2a0e86a87420bb59f35371ec957e004e2fa9fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965441"
---
# <a name="reminder-resource-type"></a>Тип ресурса reminder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Напоминание о [событии](event.md) в календаре [](calendar.md)пользователя.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|changeKey|String|Указывает версию напоминания. При каждом изменении напоминания также меняется значение **changeKey**. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|Евентендтиме|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс завершения события.|
|Диапазоне|String|Уникальный идентификатор события. Только для чтения.|
|Евентлокатион|[Location](location.md)|Место проведения события.|
|Евентстарттиме|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс начала события.|
|Евентсубжект|String|Текст в строке темы сообщения о событии.|
|Евентвеблинк|String|URL-адрес для открытия события в Outlook в Интернете.<br/><br/>Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br/><br/>Доступ к этому URL-адресу можно получить из объекта iFrame.|
|Реминдерфиретиме|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, заданные для упоминания.|

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
<!--
{
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
