---
title: Тип ресурса conditionalAccessUsers
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6214c3daacf580aaffa01a93be2b2c785c03f4fd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128584"
---
# <a name="conditionalaccessusers-resource-type"></a>Тип ресурса conditionalAccessUsers

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeUsers | Коллекция объектов string | User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers` . |
| excludeUsers | Коллекция объектов string | User IDs excluded from scope of policy and/or `GuestsOrExternalUsers` . |
| includeGroups | Коллекция объектов string | Групповые ИД в области политики, если явно не исключены, или `All` . |
| excludeGroups | Коллекция объектов string | ИД группы, исключенные из области действия политики. |
| includeRoles | Коллекция объектов string | ИД ролей в области политики, если явно не исключено, или `All` . |
| excludeRoles | Коллекция объектов string | ИД ролей, исключенные из области действия политики. |

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

