---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: outlook
author: harini84
ms.openlocfilehash: 860afaffc2ce6bcc42a4730b7672983922b066b9
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123897"
---
# <a name="responsestatus-resource-type"></a>Тип ресурса responseStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Состояние ответа участника или организатора для запроса собрания.

Вы можете получить статус ответа участника или организатора через [](event.md) **свойство responseStatus** события или свойство состояния  [участника.](attendee.md)

## <a name="properties"></a>Свойства

| Свойство | Тип           | Описание |
|:---------|:---------------|:------------|
| response | String         | Тип ответа. Возможные значения: `none`, `organizer`, `tentativelyAccepted`, `accepted`, `declined`, `notResponded`.<br><br>Разграничить `none` и `notResponded` : <br><br> `none` — с точки зрения организатора. Это значение используется, когда о состоянии участника или участника сообщается организатору собрания. <br><br> `notResponded` — с точки зрения attendde. Указывает, что участник не ответил на запрос собрания. <br><br> Клиенты могут лечить `notResponded`  ==  `none` . <br><br> Например, если участник Алекс не ответил на запрос собрания, возвращается статус ответа Алекса для этого события в календаре `notResponded` Алекса. Получение ответа Алекса из календаря любого другого участника или возврата `none` организатора. Возвращается и ответ организатора на событие в календаре `none` любого. 
| time     | DateTimeOffset | Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


