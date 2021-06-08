---
title: тип ресурса timeClockSettings
description: Представляет параметры времени для расписания.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 96ffddc0730ffaff73d21a8ab051acf9ea140ccc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786391"
---
# <a name="timeclocksettings-resource-type"></a>тип ресурса timeClockSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры времени для [расписания.](schedule.md)

## <a name="properties"></a>Свойства
|Свойство               |Тип           |Описание                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| approvedLocation | [geoCoordinates](geocoordinates.md)  |Aprroved location of the **timeClock**. |


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeClockSettings"
}-->
```json
{ 
   "approvedLocation": {

           "altitude": {"@odata.type": "microsoft.graph.GeoCoordinates"},

           "latitude": {"@odata.type": "microsoft.graph.GeoCoordinates"},

           "longitude": {"@odata.type": "microsoft.graph.GeoCoordinates"}

        }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeClockSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
