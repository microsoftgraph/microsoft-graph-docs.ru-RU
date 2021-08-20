---
title: тип ресурса yammerDeviceUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 9f5bee5edf3dbde4d889af6ecd607d3323a7c1eabc9c92a5443e174d34646bf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249673"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a>тип ресурса yammerDeviceUsageUserCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| reportRefreshDate | Дата   |
| web               | Int32  |
| WindowsPhone      | Int32  |
| AndroidPhone      | Int32  |
| iPhone            | Int32  |
| iPad              | Int32  |
| другие             | Int32  |
| reportDate        | Дата   |
| reportPeriod      | Строка |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "other": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


