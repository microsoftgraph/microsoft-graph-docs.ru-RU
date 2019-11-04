---
title: Тип ресурса Сеарчреспонсе
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7e68eae7c31486646c4b3d135881fd04fa8c7222
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938760"
---
# <a name="searchresponse-resource-type"></a>Тип ресурса Сеарчреспонсе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сеарчреспонсе содержит результаты из поискового запроса.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|хитсконтаинерс|Коллекция [сеарчхитсконтаинер](searchhitscontainer.md)|Коллекция результатов поиска.|
|searchTerms|Коллекция строк|Содержит условия поиска, отправленные в исходном поисковом запросе.|

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