---
title: Тип ресурса Ситеусажестораже
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 1ed15d4efb1c9a0fa81fdd79faeb9542d8093aab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008231"
---
# <a name="siteusagestorage-resource-type"></a>Тип ресурса Ситеусажестораже

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| Репортрефрешдате  | Дата   |
| Ситетипе           | String |
| Сторажеусединбитес | Int64  |
| reportDate         | Дата   |
| Репортпериод       | String |

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
