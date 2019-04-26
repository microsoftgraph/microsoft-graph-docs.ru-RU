---
title: Тип ресурса Скипефорбусинессактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: e59bd33b1709780bac9726ee716ef9d81ef33c1f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568161"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a>Тип ресурса Скипефорбусинессактивитикаунтс

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| Пиртопир        | Int64  |
| распределяют         | Int64  |
| участвовал      | Int64  |
| Репортрефрешдате | Дата   |
| reportDate        | Дата   |
| Репортпериод      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
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
