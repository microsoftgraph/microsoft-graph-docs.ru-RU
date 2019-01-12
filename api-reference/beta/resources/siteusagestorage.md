---
title: Тип ресурса siteUsageStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928103"
---
# <a name="siteusagestorage-resource-type"></a>Тип ресурса siteUsageStorage

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| reportRefreshDate  | Date   |
| siteType           | Строка |
| storageUsedInBytes | Int64  |
| reportDate         | Date   |
| reportPeriod       | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
