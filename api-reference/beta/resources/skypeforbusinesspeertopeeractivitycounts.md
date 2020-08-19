---
title: Тип ресурса Скипефорбусинесспиртопирактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 6bdcd96a8c6eb3dff29304bf8dc1dd8956d9063d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811044"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a>Тип ресурса Скипефорбусинесспиртопирактивитикаунтс

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| im                | Int64  |
| audio             | Int64  |
| video             | Int64  |
| аппшаринг        | Int64  |
| филетрансфер      | Int64  |
| репортрефрешдате | Дата   |
| reportDate        | Дата   |
| репортпериод      | String |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```json
{
  "im": 1024,
  "audio": 1024,
  "video": 1024,
  "appSharing": 1024,
  "fileTransfer": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
