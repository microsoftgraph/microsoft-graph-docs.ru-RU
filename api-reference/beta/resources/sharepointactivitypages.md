---
title: Тип ресурса Шарепоинтактивитипажес
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: a3d54e388d5a43489cac285a481b6ca1137aeba5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965098"
---
# <a name="sharepointactivitypages-resource-type"></a>Тип ресурса Шарепоинтактивитипажес

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| Репортрефрешдате | Дата   |
| Виситедпажекаунт  | Int64  |
| reportDate        | Дата   |
| Репортпериод      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPageCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
