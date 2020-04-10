---
title: Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир
description: Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — Аттрибутемаппингсаурце.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 88dd652e12a8ba7d5d866e2817685e0ad3a732eb
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217579"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a>Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — [аттрибутемаппингсаурце](synchronization-attributemappingsource.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|key|Строка|Имя параметра.|
|значение|[аттрибутемаппингсаурце](synchronization-attributemappingsource.md)|Значение параметра.|

## <a name="json-representation"></a>Представление JSON

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
