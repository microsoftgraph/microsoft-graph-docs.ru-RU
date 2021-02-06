---
title: Тип ресурса stringKeyAttributeMappingSourceValuePair
description: Представляет пару "ключ-значение", где ключ является строкой, а значением является attributeMappingSource.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d0bd761b64c41c930bda84b820d98501870e0c26
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135100"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a>Тип ресурса stringKeyAttributeMappingSourceValuePair

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пару "ключ-значение", где ключ является строкой, а [значением является attributeMappingSource.](synchronization-attributemappingsource.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|key|Строка|Имя параметра.|
|значение|[attributeMappingSource](synchronization-attributemappingsource.md)|Значение параметра.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


