---
title: Тип ресурса yammerGroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: a308b6180eaf91614247b0b5f47064ae7e7de2b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081477"
---
# <a name="yammergroupsactivitycounts-resource-type"></a>Тип ресурса yammerGroupsActivityCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| reportRefreshDate | Date   |
| нравится, что             | Int64  |
| учтена            | Int64  |
| чтение              | Int64  |
| reportDate        | Date   |
| reportPeriod      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
