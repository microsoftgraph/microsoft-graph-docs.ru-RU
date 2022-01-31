---
title: тип ресурса searchResponse
description: 'Представляет результаты запроса поиска и термины, используемые для запроса. '
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 956bb2b38aefdf33f3c1b7096a2e599253e7e3af
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282153"
---
# <a name="searchresponse-resource-type"></a>тип ресурса searchResponse

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет результаты запроса поиска и термины, используемые для запроса. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hitsContainers|[коллекция searchHitsContainer](searchhitscontainer.md)|Коллекция результатов поиска.|
|searchTerms|Коллекция объектов string|Содержит термины поиска, отправленные в исходном запросе поиска.|
|resultTemplates|[коллекция resultTemplate](resultTemplate.md)|Словарь resultTemplateIds и связанных с ними значений, которые включают имя и схему JSON шаблонов результатов.
|queryAlterationResponse|[alterationResponse](alterationResponse.md)|Предоставляет сведения об ответе на изменение запросов для исправления правописания.|

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
  "queryAlterationResponse": {"@odata.type": "microsoft.graph.alterationResponse"},
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"],
  "resultTemplates": [{"@odata.type":"microsoft.graph.resultTemplateDictionary"}]
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

