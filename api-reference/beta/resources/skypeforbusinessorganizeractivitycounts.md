---
title: Тип ресурса skypeForBusinessOrganizerActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 9f6c77e86f76ac2e34fb87cf8ca5b6bded35a2a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866621"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a>Тип ресурса skypeForBusinessOrganizerActivityCounts

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| обмен мгновенными сообщениями                 | Int64  |
| Ресурс         | Int64  |
| appSharing         | Int64  |
| web                | Int64  |
| dialInOut3rdParty  | Int64  |
| dialInOutMicrosoft | Int64  |
| reportRefreshDate  | Date   |
| reportDate         | Date   |
| reportPeriod       | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
