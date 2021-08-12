---
title: тип ресурса conditionalAccessLocations
description: Представляет расположения, включенные и исключенные из области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e2ad772d4e41e9244b126b8df4e0052d27a3a3d20ae9db7a974b4765eb0d190d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205929"
---
# <a name="conditionalaccesslocations-resource-type"></a>тип ресурса conditionalAccessLocations

Пространство имен: microsoft.graph

Представляет расположения, включенные и исключенные из области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeLocations | Коллекция String | Определения местоположения в области политики, если явно не исключены, `All` или `AllTrusted` . |
| excludeLocations | Коллекция строк | ИД расположения исключены из области политики. |

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

