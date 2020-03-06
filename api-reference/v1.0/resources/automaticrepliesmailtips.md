---
title: Тип ресурса Аутоматикреплиесмаилтипс
description: Подсказки о любых автоматических ответах, настроенных в почтовом ящике.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7d7c5c6a3560435c4e61a8953887f5b6b61324
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532043"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Тип ресурса Аутоматикреплиесмаилтипс

Пространство имен: microsoft.graph


[Подсказки](../resources/mailtips.md) о любых автоматических ответах, настроенных в почтовом ящике.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:-----|:-----|:-----|
| message | String | Сообщение автоматического ответа. |
| мессажелангуаже | [localeInfo](../resources/localeinfo.md) | Язык, на котором находится сообщение с автоматическим ответом. |
| счедуледендтиме | [dateTimeTimeZone](../resources/datetimetimezone.md) | Дата и время завершения установки автоматических ответов. |
| счедуледстарттиме | [dateTimeTimeZone](../resources/datetimetimezone.md) | Дата и время начала набора автоматических ответов. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
