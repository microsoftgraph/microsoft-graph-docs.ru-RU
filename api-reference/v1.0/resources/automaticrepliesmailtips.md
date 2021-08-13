---
title: тип ресурса automaticRepliesMailTips
description: MailTips о любых автоматических ответах, которые были настроены на почтовом ящике.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 98f509f1bf8010e40924de0a525d876f2a08e9e08df0a9b5826e98a00f14696c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54147044"
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

