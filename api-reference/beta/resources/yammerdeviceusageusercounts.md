---
title: Тип ресурса yammerDeviceUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 878fe76fa65d5f8b12be382a161ace9271c6e415
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981541"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a>Тип ресурса yammerDeviceUsageUserCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| reportRefreshDate | Date   |
| web               | Int32  |
| windowsPhone      | Int32  |
| androidPhone      | Int32  |
| "iPhone";            | Int32  |
| "iPad";              | Int32  |
| другие             | Int32  |
| reportDate        | Date   |
| reportPeriod      | String |

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
