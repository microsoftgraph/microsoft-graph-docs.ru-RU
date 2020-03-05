---
title: Тип ресурса Яммерграупсактивитиграупкаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 426b3e2a6be72c0cc87d4c284b56fd83b1c12141
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518982"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a>Тип ресурса Яммерграупсактивитиграупкаунтс

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание |
| :---------------- | :----- | :---------- |
| репортрефрешдате | Дата   |             |
| total             | Int64  |             |
| ASP            | Int64  |             |
| reportDate        | Дата   |             |
| репортпериод      | String |             |

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
