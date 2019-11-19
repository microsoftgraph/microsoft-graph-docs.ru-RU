---
title: Тип ресурса Сеарчреспонсе
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6b433e5aba652a9f68d017975e0651edac4e2ffb
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703997"
---
# <a name="searchresponse-resource-type"></a>Тип ресурса Сеарчреспонсе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сеарчреспонсе содержит результаты из поискового запроса.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

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