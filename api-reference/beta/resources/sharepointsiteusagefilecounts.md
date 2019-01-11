---
title: Тип ресурса sharePointSiteUsageFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: b304a5bb519f8ffb2a23087b2ea38fd12fde6fab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836129"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a>Тип ресурса sharePointSiteUsageFileCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| reportRefreshDate | Date   |
| siteType          | Строка |
| total             | Int64  |
| активных            | Int64  |
| reportDate        | Date   |
| reportPeriod      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
