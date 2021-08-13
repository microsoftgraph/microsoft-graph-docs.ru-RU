---
title: тип ресурса searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5d28f3a2a423947eaf27a5b6878607d6efac6dda3dd6d2f01907621b17177732
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149676"
---
# <a name="searchquery-resource-type"></a>тип ресурса searchQuery

Пространство имен: microsoft.graph

Представляет поисковый запрос, содержащий термины поиска и необязательные фильтры.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|queryString|String|Поисковый запрос, содержащий термины поиска. Обязательный элемент.|

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
  "queryString": "String"
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

