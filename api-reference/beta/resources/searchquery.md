---
title: тип ресурса searchQuery
description: searchQuery
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0c437bcb8fd7462d8c4bc85514c40d47311155de
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589319"
---
# <a name="searchquery-resource-type"></a>тип ресурса searchQuery

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Представляет поисковый запрос, содержащий термины поиска и необязательные фильтры.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|queryString|Строка|Поисковый запрос, содержащий термины поиска. Обязательный аргумент.|
|queryTemplate|String|Предоставляет способ украсить строку запроса. Поддерживает переменные KQL и запроса. Необязательно.|
|query_string (неподготовленный)|[searchQueryString](searchquerystring.md)|Теперь это свойство **queryString заменяется** . Поисковый запрос, содержащий термины поиска.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "queryString": "String",
  "queryTemplate": "String",
  "query_string": {"@odata.type": "microsoft.graph.searchQueryString"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

