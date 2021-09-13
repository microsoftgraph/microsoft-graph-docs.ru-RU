---
title: тип ресурса skypeForBusinessActivityCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 8591596604e53d077f2f966dc794c7f346f42c9b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074551"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a>тип ресурса skypeForBusinessActivityCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| peerToPeer        | Int64  |
| организовано         | Int64  |
| участие      | Int64  |
| reportRefreshDate | Дата   |
| reportDate        | Дата   |
| reportPeriod      | String |

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


