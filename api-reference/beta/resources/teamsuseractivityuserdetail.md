---
title: Тип ресурса teamsUserActivityUserDetail
description: Ниже приведен representaion JSON ресурса.
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081479"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>Тип ресурса teamsUserActivityUserDetail

## <a name="properties"></a>Свойства

| Свойство                | Тип              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Date              |
| userPrincipalName       | String            |
| lastActivityDate        | Date              |
| isDeleted               | Логический           |
| deletedDate             | Date              |
| assignedProducts        | Коллекция String |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | Логический           |
| reportPeriod            | String            |

## <a name="json-representation"></a>Представление JSON

Ниже приведен representaion JSON ресурса.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
