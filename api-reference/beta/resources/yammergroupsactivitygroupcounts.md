---
title: Тип ресурса Яммерграупсактивитиграупкаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 64947a1d151cab3dca14f4f232671242e1a985cc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342732"
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
