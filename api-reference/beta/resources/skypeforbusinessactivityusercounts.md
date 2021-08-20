---
title: тип ресурса skypeForBusinessActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 575085ab78a8e3da81f15c525e166ca5f6f9789072e30e930f3c76ec8f273fe1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212929"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a>тип ресурса skypeForBusinessActivityUserCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| peerToPeer        | Int64  |
| организовано         | Int64  |
| участие      | Int64  |
| reportRefreshDate | Дата   |
| reportDate        | Дата   |
| reportPeriod      | Строка |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
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


