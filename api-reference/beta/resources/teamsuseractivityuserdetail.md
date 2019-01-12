---
title: Тип ресурса teamsUserActivityUserDetail
description: Ниже приведен representaion JSON ресурса.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913431"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>Тип ресурса teamsUserActivityUserDetail

## <a name="properties"></a>Свойства

| Свойство                | Тип              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Date              |
| userPrincipalName       | Строка            |
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
