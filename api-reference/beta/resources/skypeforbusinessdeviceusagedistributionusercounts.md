---
title: Тип ресурса Скипефорбусинессдевицеусажедистрибутионусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: c0134bedc15de07d89709a623b6a31a8f53ac5fe
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808615"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a>Тип ресурса Скипефорбусинессдевицеусажедистрибутионусеркаунтс

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
| репортпериод      | String |

## <a name="json-representation"></a>Представление в формате JSON

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
