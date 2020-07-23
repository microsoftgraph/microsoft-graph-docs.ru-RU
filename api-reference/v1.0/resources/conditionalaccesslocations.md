---
title: Тип ресурса Кондитионалакцесслокатионс
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5378764f36bf5fed858755a475fd85a400a2fed
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384678"
---
# <a name="conditionalaccesslocations-resource-type"></a>Тип ресурса Кондитионалакцесслокатионс

Пространство имен: microsoft.graph

Представляет расположения, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| инклуделокатионс | Коллекция String | Идентификаторы расположений в области применения политики, если явно не исключены, `All` или `AllTrusted` . |
| ексклуделокатионс | Коллекция String | Идентификаторы расположений, исключенные из области применения политики. |

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
