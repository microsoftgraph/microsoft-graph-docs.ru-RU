---
title: Тип ресурса Сеарчхитсконтаинер
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7bc36dc49a944de4a12decbf3b0b77a3c203eb21
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938718"
---
# <a name="searchhitscontainer-resource-type"></a>Тип ресурса Сеарчхитсконтаинер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет список результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|успешных|Коллекция [сеарчхит](searchhit.md)|Енкасулате результаты поиска.|
|морересултсаваилабле|Логический|Предоставляет сведения, если доступны дополнительные результаты. В этом случае можно увеличить смещение "от" и "до".|
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