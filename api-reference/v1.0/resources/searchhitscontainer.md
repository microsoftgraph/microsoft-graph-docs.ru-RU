---
title: Тип ресурса Сеарчхитсконтаинер
description: Представляет список результатов поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f32fa198624c04da6eadfc828b60350164cbdddc
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378059"
---
# <a name="searchhitscontainer-resource-type"></a>Тип ресурса Сеарчхитсконтаинер

Пространство имен: microsoft.graph

Представляет список результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|успешных|Коллекция [сеарчхит](searchhit.md)|Коллекция результатов поиска.|
|морересултсаваилабле|Boolean|Предоставляет сведения, если доступны дополнительные результаты. На основе этих сведений вы можете соответствующим образом настроить свойства **from** и **size** для [сеарчрекуест](searchrequest.md) .|
|total|Int32|Общее число результатов. Note — это не количество результатов на странице, но общее количество результатов, удовлетворяющих запросу.|


## <a name="json-representation"></a>Представление в формате JSON

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


