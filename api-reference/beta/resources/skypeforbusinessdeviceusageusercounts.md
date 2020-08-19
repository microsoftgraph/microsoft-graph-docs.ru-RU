---
title: Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 01867d92037f3bf80a7db2c25cc96a967ac560cd
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808713"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a>Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| репортрефрешдате | Дата   |
| под           | Int64  |
| windowsPhone      | Int64  |
| андроидфоне      | Int64  |
| iPhone            | Int64  |
| iPad              | Int64  |
| reportDate        | Дата   |
| репортпериод      | String |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "windows": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
