---
title: тип ресурса skypeForBusinessOrganizerActivityCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 4b67f7db5e726756755f861fc29665a1c36266d1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091043"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a>тип ресурса skypeForBusinessOrganizerActivityCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| im                 | Int64  |
| audioVideo         | Int64  |
| appSharing         | Int64  |
| web                | Int64  |
| dialInOut3rdParty  | Int64  |
| dialInOutMicrosoft | Int64  |
| reportRefreshDate  | Дата   |
| reportDate         | Дата   |
| reportPeriod       | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "dialInOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


