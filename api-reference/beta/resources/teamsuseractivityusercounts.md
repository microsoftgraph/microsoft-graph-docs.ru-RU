---
title: Тип ресурса Теамсусерактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f0b6d9d77518b6e40a5793c6715bfbae69600f3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964363"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>Тип ресурса Теамсусерактивитюсеркаунтс

## <a name="properties"></a>Свойства

| Свойство            | Тип   |
| :------------------ | :----- |
| Репортрефрешдате   | Дата   |
| reportDate          | Дата   |
| Теамчатмессажес    | Int64  |
| Приватечатмессажес | Int64  |
| calls               | Int64  |
| meetings            | Int64  |
| Осерактионс        | Int64  |
| Репортпериод        | String |

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
