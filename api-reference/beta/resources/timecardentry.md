---
title: тип ресурса timeCardEntry
description: Представляет определенную запись с химкаром.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d09b324b4d43765f05de789129021e2eb1f24789
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786411"
---
# <a name="timecardentry-resource-type"></a>тип ресурса timeCardEntry

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенную [запись timeCard.](timecard.md)

## <a name="properties"></a>Свойства
|Свойство               |Тип           |Описание                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| clockInEvent       |[timeCardEvent](timecardevent.md)    | Событие с часовой стрелкой **timeCard**.|
| clockOutEvent                 |[timeCardEvent](timecardevent.md)  |Событие clock-out **timeCard**. |
| перерывы    |[коллекция timeCardBreak](timecardbreak.md)    |Список перерывов, связанных с **timeCard**.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEntry"
}-->
```json
{
   "clockInEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "clockOutEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "string",
             "contentType": "text"
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
   ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timecardentry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
