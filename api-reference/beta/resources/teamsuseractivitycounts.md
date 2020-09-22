---
title: Тип ресурса Теамсусерактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 68eb66cbd0e076d9cf2559170fee4c81dca1e65c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046344"
---
# <a name="teamsuseractivitycounts-resource-type"></a>Тип ресурса Теамсусерактивитикаунтс

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство            | Тип   |
| :------------------ | :----- |
| репортрефрешдате   | Дата   |
| reportDate          | Дата   |
| теамчатмессажес    | Int64  |
| приватечатмессажес | Int64  |
| calls               | Int64  |
| meetings            | Int64  |
| репортпериод        | Строка |


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


