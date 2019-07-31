---
title: Тип ресурса Скипефорбусинессактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c4f97f8377ec5693be1cc477ab40119675a24908
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008203"
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
