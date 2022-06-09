---
title: Тип ресурса automaticRepliesMailTips
description: Подсказки об автоматических ответах, которые были настроены в почтовом ящике.
ms.localizationpriority: medium
author: abheek-das
ms.prod: mail
doc_type: resourcePageType
ms.openlocfilehash: 9d9350df4929bb6fbf428a229812df206e658363
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971275"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Тип ресурса automaticRepliesMailTips

Пространство имен: microsoft.graph


[Подсказки об](../resources/mailtips.md) автоматических ответах, которые были настроены в почтовом ящике.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:-----|:-----|:-----|
| message | String | Автоматическое ответное сообщение. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | Язык, на котором находится автоматическое ответное сообщение. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | Дата и время завершения автоматических ответов. |
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

