---
title: Тип ресурса rankedEmailAddress
description: Представляет ранжированные адреса электронной почты.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: AAmatino
ms.openlocfilehash: 2723009cc44680e98b9c8b5a685c06846bb9abd7
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176314"
---
# <a name="rankedemailaddress-resource-type"></a>Тип ресурса rankedEmailAddress

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ранжированные адреса электронной почты.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|string|Адрес электронной почты.|
|rank|double|Ранг адреса электронной почты. Ранг используется в качестве ключа сортировки относительно других возвращаемых результатов. Более высокое значение соответствует более актуальному результату. Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


