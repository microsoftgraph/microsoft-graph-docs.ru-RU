---
title: Тип ресурса Аутоматикреплиесмаилтипс
description: Подсказки о любых автоматических ответах, настроенных в почтовом ящике.
localization_priority: Normal
ms.openlocfilehash: bb477979b975996f70e4b8ac624befab7f254f46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569454"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Тип ресурса Аутоматикреплиесмаилтипс


[Подсказки](../resources/mailtips.md) о любых автоматических ответах, настроенных в почтовом ящике.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:-----|:-----|:-----|
| message | String | Сообщение автоматического ответа. |
| Мессажелангуаже | [localeInfo](../resources/localeinfo.md) | Язык, на котором находится сообщение с автоматическим ответом. |
| Счедуледендтиме | [dateTimeTimeZone](../resources/datetimetimezone.md) | Дата и время завершения установки автоматических ответов. |
| Счедуледстарттиме | [dateTimeTimeZone](../resources/datetimetimezone.md) | Дата и время начала набора автоматических ответов. |

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
