---
title: Тип ресурса automaticRepliesMailTips
description: Почтовые подсказки о автоматические ответы, которые были настроены для почтового ящика.
localization_priority: Normal
ms.openlocfilehash: 7eb9d57da427090c554e111ae6ba1eeb369437ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513678"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Тип ресурса automaticRepliesMailTips

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliesmailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
