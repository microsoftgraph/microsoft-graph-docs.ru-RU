---
title: тип ресурса searchResponse
description: Описание searchResponse
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e071126b95cf0f82143c22f4523adcad640cb7df66718858a722e9f120177edc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246565"
---
# <a name="searchresponse-resource-type"></a>тип ресурса searchResponse

Пространство имен: microsoft.graph

Представляет результаты запроса поиска и термины, используемые для запроса. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hitsContainers|[коллекция searchHitsContainer](searchhitscontainer.md)|Коллекция результатов поиска.|
|searchTerms|Коллекция String|Содержит термины поиска, отправленные в исходном запросе поиска.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

