---
title: тип ресурса searchHitsContainer
description: Представляем список результатов поиска.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ebd8440c5f417786c002f074ef90646f156549d4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137541"
---
# <a name="searchhitscontainer-resource-type"></a>тип ресурса searchHitsContainer

Пространство имен: microsoft.graph

Представляем список результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hits|[коллекция searchHit](searchhit.md)|Коллекция результатов поиска.|
|moreResultsAvailable|Логический|Предоставляет сведения, если доступны дополнительные результаты. На основании этих сведений  можно  соответствующим образом настроить свойства [searchRequest](searchrequest.md) с размером и размером.|
|total|Int32|Общее количество результатов. Обратите внимание, что это не количество результатов на странице, а общее число результатов, удовлетворяющих запрос.|


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


