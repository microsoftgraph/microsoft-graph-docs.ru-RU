---
title: Тип ресурса Ситеусажестораже
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583202"
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
