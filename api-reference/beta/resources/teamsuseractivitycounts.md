---
title: Тип ресурса Теамсусерактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582922"
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
