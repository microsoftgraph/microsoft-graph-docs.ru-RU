---
title: Тип ресурса Яммерграупсактивитиграупкаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 4c342686ce2397a5d3b1dd697002fb44e16f3b11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006922"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a>Тип ресурса Яммерграупсактивитиграупкаунтс

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание |
| :---------------- | :----- | :---------- |
| Репортрефрешдате | Дата   |             |
| total             | Int64  |             |
| ASP            | Int64  |             |
| reportDate        | Дата   |             |
| Репортпериод      | String |             |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts"
} -->

```json
{
  "reportRefreshDate": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "String", 
  "reportPeriod": "String"
}
```
