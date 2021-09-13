---
title: тип ресурса mailboxUsageStorage
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4e16a69e5ae266607c4d257e4d32901a20af6975
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59119991"
---
# <a name="mailboxusagestorage-resource-type"></a>тип ресурса mailboxUsageStorage

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| reportRefreshDate  | Дата   |
| storageUsedInBytes | Int64  |
| reportDate         | Дата   |
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


