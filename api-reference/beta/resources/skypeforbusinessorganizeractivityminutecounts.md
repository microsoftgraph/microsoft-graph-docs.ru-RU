---
title: тип ресурса skypeForBusinessOrganizerActivityMinuteCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: ba19256ad7359699e881aa47fb0e1eaaad2f80250ad00fd13a775614ff10e923
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241270"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a>тип ресурса skypeForBusinessOrganizerActivityMinuteCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| audioVideo         | Int64  |
| dialInMicrosoft    | Int64  |
| dialOutMicrosoft   | Int64  |
| reportRefreshDate  | Дата   |
| reportDate         | Дата   |
| reportPeriod       | Строка |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```json
{
  "audioVideo": 1024,
  "dialInMicrosoft": 1024,
  "dialOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


