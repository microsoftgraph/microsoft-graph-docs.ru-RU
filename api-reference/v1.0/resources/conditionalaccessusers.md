---
title: Тип ресурса conditionalAccessUsers
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8f75eb86ab9627b2cb9d507de9321743524203b3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129774"
---
# <a name="conditionalaccessusers-resource-type"></a>Тип ресурса conditionalAccessUsers

Пространство имен: microsoft.graph

Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeUsers | Коллекция String | User IDs in scope of policy unless explicitly excluded, or `None` `All` or or `GuestsOrExternalUsers` . |
| excludeUsers | Коллекция String | ИД пользователей, исключенных из области действия политики и/или `GuestsOrExternalUsers` . |
| includeGroups | Коллекция String | Групповые ИД в области политики, если явно не исключены, или `All` . |
| excludeGroups | Коллекция String | ИД группы, исключенные из области действия политики. |
| includeRoles | Коллекция String | ИД ролей в области политики, если явно не исключено, или `All` . |
| excludeRoles | Коллекция String | ИД ролей, исключенные из области действия политики. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeUsers",
    "excludeUsers",
    "includeGroups",
    "excludeGroups",
    "includeRoles",
    "excludeRoles"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessUsers",
  "baseType": null
}-->

```json
{
  "excludeGroups": ["String"],
  "excludeRoles": ["String"],
  "excludeUsers": ["String"],
  "includeGroups": ["String"],
  "includeRoles": ["String"],
  "includeUsers": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessUsers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

