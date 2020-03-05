---
title: Тип ресурса Теамсусерактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3066877d109e7dd61243b7cd2f4c105b03c0c533
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519829"
---
# <a name="teamsuseractivitycounts-resource-type"></a>Тип ресурса Теамсусерактивитикаунтс

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство            | Тип   |
| :------------------ | :----- |
| репортрефрешдате   | Дата   |
| reportDate          | Дата   |
| теамчатмессажес    | Int64  |
| приватечатмессажес | Int64  |
| calls               | Int64  |
| meetings            | Int64  |
| репортпериод        | String |


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
