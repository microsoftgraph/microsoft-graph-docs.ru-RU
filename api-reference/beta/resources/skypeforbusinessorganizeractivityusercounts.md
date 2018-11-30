---
title: Тип ресурса skypeForBusinessOrganizerActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 0e0b6838b58b4a3fab9a62351446bf26fc50bfbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079814"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a>Тип ресурса skypeForBusinessOrganizerActivityUserCounts

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
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
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
