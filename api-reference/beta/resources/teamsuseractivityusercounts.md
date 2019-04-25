---
title: Тип ресурса Теамсусерактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582915"
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
