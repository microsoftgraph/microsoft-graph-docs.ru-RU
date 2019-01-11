---
title: Тип ресурса automaticRepliesMailTips
description: Почтовые подсказки о автоматические ответы, которые были настроены для почтового ящика.
localization_priority: Normal
ms.openlocfilehash: bb477979b975996f70e4b8ac624befab7f254f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816277"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Тип ресурса automaticRepliesMailTips


[Почтовые подсказки](../resources/mailtips.md) о автоматические ответы, которые были настроены для почтового ящика.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:-----|:-----|:-----|
| message | String | Сообщение автоматического ответа. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | Язык, сообщение автоматического ответа. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | Дата и время окончания устанавливаются автоматические ответы. |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | Дата и время автоматические ответы чтобы начать. |

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
