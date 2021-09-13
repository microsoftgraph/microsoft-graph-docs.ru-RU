---
title: тип ресурса conditionalAccessLocations
description: Представляет расположения, включенные и исключенные из области политики.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 68804b5728fd058d2502ac041a24c3a218692b93
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109249"
---
# <a name="conditionalaccesslocations-resource-type"></a>тип ресурса conditionalAccessLocations

Пространство имен: microsoft.graph

Представляет расположения, включенные и исключенные из области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeLocations | Коллекция String | Определения местоположения в области политики, если явно не исключены, `All` или `AllTrusted` . |
| excludeLocations | Коллекция String | ИД расположения исключены из области политики. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

## <a name="relationships"></a>Отношения

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

