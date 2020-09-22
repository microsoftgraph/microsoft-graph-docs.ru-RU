---
title: Тип ресурса Теамсусерактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3982b679802a2ca80eac5fe4e8f76fee91bbf1d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046351"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>Тип ресурса Теамсусерактивитюсеркаунтс

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
| осерактионс        | Int64  |
| репортпериод        | Строка |

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


