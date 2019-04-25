---
title: Тип ресурса Скипефорбусинессдевицеусажедистрибутионусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 3658bec2d99c5098b970e35240221dbf954beba6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581263"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a>Тип ресурса Скипефорбусинессдевицеусажедистрибутионусеркаунтс

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| Репортрефрешдате | Дата   |
| под           | Int64  |
| windowsPhone      | Int64  |
| Андроидфоне      | Int64  |
| iPhone            | Int64  |
| iPad              | Int64  |
| Репортпериод      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportPeriod": "String"
}
```
