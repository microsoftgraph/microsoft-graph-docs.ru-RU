---
title: Тип ресурса stringKeyObjectValuePair
description: Представляет пару "ключ-значение", где ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который должен иметь свойство с именем, которое `value` является допустимым объектом JSON.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 535e9f104f42771e6f6c182769f0a5e1f68169b6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137069"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>Тип ресурса stringKeyObjectValuePair

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пару "ключ-значение", где ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который должен иметь свойство с именем, которое `value` является допустимым объектом JSON.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|key|Строка|Ключ.|
|значение|Json|Произвольный объект JSON.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


