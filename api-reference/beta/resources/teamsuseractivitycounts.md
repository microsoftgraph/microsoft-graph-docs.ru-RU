---
title: Тип ресурса Теамсусерактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9e1a40d962ded7825b72d31675cefb9869750866
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007623"
---
# <a name="teamsuseractivitycounts-resource-type"></a>Тип ресурса Теамсусерактивитикаунтс

## <a name="properties"></a>Свойства

| Свойство            | Тип   |
| :------------------ | :----- |
| Репортрефрешдате   | Дата   |
| reportDate          | Дата   |
| Теамчатмессажес    | Int64  |
| Приватечатмессажес | Int64  |
| calls               | Int64  |
| meetings            | Int64  |
| Репортпериод        | String |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
