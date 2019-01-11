---
title: Тип ресурса teamsUserActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8a48a80992d8370a3b6b198862a3af901737fa04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836661"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>Тип ресурса teamsUserActivityUserCounts

## <a name="properties"></a>Свойства

| Свойство            | Тип   |
| :------------------ | :----- |
| reportRefreshDate   | Date   |
| reportDate          | Date   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| звонки               | Int64  |
| собрания            | Int64  |
| otherActions        | Int64  |
| reportPeriod        | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
