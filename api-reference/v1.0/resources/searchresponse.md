---
title: тип ресурса searchResponse
description: Описание searchResponse
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b7d5668a86204e95e3f0f5e024ec985f98027ac9
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878654"
---
# <a name="searchresponse-resource-type"></a>тип ресурса searchResponse

Пространство имен: microsoft.graph

Представляет результаты запроса поиска и термины, используемые для запроса. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hitsContainers|[коллекция searchHitsContainer](searchhitscontainer.md)|Коллекция результатов поиска.|
|resultTemplates|[коллекция resultTemplate](resulttemplate.md)|Словарь **resultTemplateIds** и связанных с ними значений, которые включают имя и схему JSON шаблонов результатов.|
|searchTerms|Коллекция объектов string|Содержит термины поиска, отправленные в исходном запросе поиска.|
|queryAlterationResponse|[alterationResponse](alterationresponse.md)|Предоставляет сведения, связанные с исправлениями орфографии в ответе на изменения.|

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
  "queryAlterationResponse": {"@odata.type": "microsoft.graph.alterationResponse"},
  "resultTemplates": [{"@odata.type":"microsoft.graph.resultTemplateDictionary"}],
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

