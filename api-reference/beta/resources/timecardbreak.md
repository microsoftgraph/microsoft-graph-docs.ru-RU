---
title: тип ресурса timeCardBreak
description: Представляет определенный разрыв химкарта.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 509667ec1fad41f956ee5ee6d6a4371b8d17fc2e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786394"
---
# <a name="timecardbreak-resource-type"></a>тип ресурса timeCardBreak

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный [разрыв timeCard.](timecard.md)

## <a name="properties"></a>Свойства
|Свойство               |Тип           |Описание                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| breakId                   |`Edm.string`  |ID **timeCardBreak**.|
| начать                 |[timeCardEvent](timecardevent.md)    | Событие начала **timeCardBreak**.|
| end                   |[timeCardEvent](timecardevent.md)    | Событие начала **timeCardBreak**.|
| notes                 |[itemBody](itembody.md)  | Заметки о **timeCardBreak**.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardBreak"
}-->
```json
{
    "breakId":"string",
    "notes":{
        "content": "string",
        "contentType": "string"
    },
    "start":{
        "dateTime":"String (timestamp)",
        "atApprovedLocation":true,
        "notes":{
            "content": "string",
            "contentType": "text"
        },
    },
    "end":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardBreak resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
