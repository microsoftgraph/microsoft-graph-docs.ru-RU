---
title: Тип ресурса Скипефорбусинессактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 1b61e4704ebbab9bea813bfe96c0ae9639fdb1b6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807397"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a>Тип ресурса Скипефорбусинессактивитикаунтс

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| пиртопир        | Int64  |
| распределяют         | Int64  |
| участвовал      | Int64  |
| репортрефрешдате | Дата   |
| reportDate        | Дата   |
| репортпериод      | String |

## <a name="json-representation"></a>Представление в формате JSON

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
