---
title: Тип ресурса mailboxUsageStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: dcabfab0e8a64f2d74442f7d7464708501a59b95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840742"
---
# <a name="mailboxusagestorage-resource-type"></a>Тип ресурса mailboxUsageStorage

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| reportRefreshDate  | Date   |
| storageUsedInBytes | Int64  |
| reportDate         | Date   |
| reportPeriod       | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
