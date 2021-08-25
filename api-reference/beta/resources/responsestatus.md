---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: harini84
ms.openlocfilehash: f7559f90f1bef35601136e944d57bfec4951cdbf
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514086"
---
# <a name="responsestatus-resource-type"></a>Тип ресурса responseStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Состояние ответа участника или организатора для запроса собрания.

Вы можете получить статус ответа участника или организатора через [](event.md) **свойство responseStatus** события или свойство состояния  [участника.](attendee.md)

## <a name="properties"></a>Свойства

| Свойство | Тип           | Описание |
|:---------|:---------------|:------------|
| response | String         | Тип ответа. Возможные значения: `none`, `organizer`, `tentativelyAccepted`, `accepted`, `declined`, `notResponded`.<br><br>Чтобы различать и : например, если участник Алекс не ответил на запрос собрания, получение статуса ответа Алекса для этого события в календаре `none` `notResponded` Алекс `notResponded` возвращается . Получение ответа Алекса из календаря любого другого участника или возврата `none` организатора. Возвращается и ответ организатора на событие в календаре `none` любого. 
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


