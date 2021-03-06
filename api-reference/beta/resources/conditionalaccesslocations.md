---
title: Тип ресурса conditionalAccessLocations
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 153d64d32015fcd6119a4d880bbc786905c39b9f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132404"
---
# <a name="conditionalaccesslocations-resource-type"></a>Тип ресурса conditionalAccessLocations

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расположения, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeLocations | Коллекция объектов string | ИД расположения в области политики, если явно не исключены, `All` или `AllTrusted` . |
| excludeLocations | Коллекция объектов string | ИД расположения, исключенные из области действия политики. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

## <a name="relationships"></a>Связи

Отсутствуют.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeLocations",
    "excludeLocations"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessLocations",
  "baseType": null
}-->

```json
{
  "excludeLocations": ["String"],
  "includeLocations": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessLocations resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

