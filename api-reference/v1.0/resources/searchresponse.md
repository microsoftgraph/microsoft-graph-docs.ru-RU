---
title: Тип ресурса Сеарчреспонсе
description: Описание Сеарчреспонсе
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8582da8daf604952807e05376d98dabf16267052
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377780"
---
# <a name="searchresponse-resource-type"></a>Тип ресурса Сеарчреспонсе

Пространство имен: microsoft.graph

Представляет результаты из поискового запроса и термины, используемые для запроса. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|хитсконтаинерс|Коллекция [сеарчхитсконтаинер](searchhitscontainer.md)|Коллекция результатов поиска.|
|searchTerms|Коллекция String|Содержит условия поиска, отправленные в исходном поисковом запросе.|

## <a name="json-representation"></a>Представление в формате JSON

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

