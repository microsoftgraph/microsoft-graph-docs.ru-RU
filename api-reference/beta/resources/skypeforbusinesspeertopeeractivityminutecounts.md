---
title: Тип ресурса skypeForBusinessPeerToPeerActivityMinuteCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 695c2fc57ab9d105b2576a9228ccc58d74b0094d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851620"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a>Тип ресурса skypeForBusinessPeerToPeerActivityMinuteCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| audio             | Int64  |
| video             | Int64  |
| reportRefreshDate | Date   |
| reportDate        | Date   |
| reportPeriod      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```json
{
  "audio": 1024, 
  "video": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
