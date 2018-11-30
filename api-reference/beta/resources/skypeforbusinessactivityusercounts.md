---
title: Тип ресурса skypeForBusinessActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: eee736958540f2a3fb42cf3c76a37da4ebe78afd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082832"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a>Тип ресурса skypeForBusinessActivityUserCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| peerToPeer        | Int64  |
| упорядоченные         | Int64  |
| являлся      | Int64  |
| reportRefreshDate | Date   |
| reportDate        | Date   |
| reportPeriod      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
