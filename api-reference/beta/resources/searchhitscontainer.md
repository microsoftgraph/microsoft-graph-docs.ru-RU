---
title: Тип ресурса Сеарчхитсконтаинер
description: Представляет список результатов поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a2d120722179cb0fd771a84f867948a7fbfffdd4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192788"
---
# <a name="searchhitscontainer-resource-type"></a>Тип ресурса Сеарчхитсконтаинер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет список результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|успешных|Коллекция [сеарчхит](searchhit.md)|Коллекция результатов поиска.|
|морересултсаваилабле|Логическое|Предоставляет сведения, если доступны дополнительные результаты. На основе этих сведений вы можете соответствующим образом настроить свойства **from** и **size** для [сеарчрекуест](searchrequest.md) .|
|total|Int32|Общее число результатов. Note — это не количество результатов на странице, но общее количество результатов, удовлетворяющих запросу.|
|Aggregations|Коллекция [сеарчаггрегатион](searchaggregation.md)|Содержит коллекцию агрегатов, вычисляемых на основе предоставленного [аггрегатионоптион](aggregationoption.md) , указанного в запросе.|

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
  "total": 1024,
  "aggregations": [{"@odata.type": "microsoft.graph.searchAggregation"}]
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


