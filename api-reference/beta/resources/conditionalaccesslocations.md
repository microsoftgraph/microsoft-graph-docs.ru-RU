---
title: Тип ресурса Кондитионалакцесслокатионс
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6997664eb131664bcaaf571398ed393fb13c987c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638570"
---
# <a name="conditionalaccesslocations-resource-type"></a>Тип ресурса Кондитионалакцесслокатионс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расположения, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| инклуделокатионс | Коллекция строк | Идентификаторы расположений в области применения политики, если `All`явно не `AllTrusted`исключены, или. |
| ексклуделокатионс | Коллекция строк | Идентификаторы расположений, исключенные из области применения политики. |

## <a name="json-representation"></a>Представление JSON

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