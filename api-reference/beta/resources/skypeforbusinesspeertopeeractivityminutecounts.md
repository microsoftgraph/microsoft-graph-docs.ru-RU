---
title: Тип ресурса skypeForBusinessPeerToPeerActivityMinuteCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 5377e8d8f2ec145f5aee590409206de75e915d9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081656"
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
