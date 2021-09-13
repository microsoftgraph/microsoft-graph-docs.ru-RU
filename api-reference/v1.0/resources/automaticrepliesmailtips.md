---
title: тип ресурса automaticRepliesMailTips
description: MailTips о любых автоматических ответах, которые были настроены на почтовом ящике.
ms.localizationpriority: medium
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3e9904fe54d14fe707f4917934b81750aa9ec5fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089867"
---
# <a name="automaticrepliesmailtips-resource-type"></a>тип ресурса automaticRepliesMailTips

Пространство имен: microsoft.graph


[MailTips](../resources/mailtips.md) о любых автоматических ответах, которые были настроены на почтовом ящике.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:-----|:-----|:-----|
| message | String | Автоматическое сообщение ответа. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | Язык, на который находится автоматическое сообщение ответа. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | Дата и время, когда автоматические ответы должны быть засвечив. |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | Дата и время начала автоматических ответов. |

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

