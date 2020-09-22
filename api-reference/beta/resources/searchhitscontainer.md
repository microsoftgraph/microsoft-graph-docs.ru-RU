---
title: Тип ресурса Сеарчхитсконтаинер
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d314fcdd2a62be5aea05bed3b2a9e1881f95c3d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985799"
---
# <a name="searchhitscontainer-resource-type"></a>Тип ресурса Сеарчхитсконтаинер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет список результатов поиска.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|успешных|Коллекция [сеарчхит](searchhit.md)|Енкасулате результаты поиска.|
|морересултсаваилабле|Boolean|Предоставляет сведения, если доступны дополнительные результаты. В этом случае можно увеличить смещение "от" и "до".|
|total|Int32|Общее число результатов. Обратите внимание, что это не количество результатов на странице, а общее количество результатов, удовлетворяющих запросу.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHitsContainer",
  "baseType": null
}-->

```json
{
  "hits": [{"@odata.type": "microsoft.graph.searchHit"}],
  "moreResultsAvailable": true,
  "total": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHitsContainer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

