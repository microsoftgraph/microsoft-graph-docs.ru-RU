---
title: тип ресурса sharePointSiteUsagePages
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 1a1378bbe4ebaf1809aa641b22cde439f50d830b016b7cc393842f21cecbe029
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246088"
---
# <a name="sharepointsiteusagepages-resource-type"></a>тип ресурса sharePointSiteUsagePages

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| reportRefreshDate | Дата   |
| siteType          | Строка |
| pageViewCount     | Int64  |
| reportDate        | Дата   |
| reportPeriod      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteType": "String",
  "pageViewCount": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


