---
title: тип ресурса conditionalAccessUsers
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5d425a2c5387f940c1e6d475a5bac26c85ebfaaf
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162099"
---
# <a name="conditionalaccessusers-resource-type"></a>тип ресурса conditionalAccessUsers

Пространство имен: microsoft.graph

Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeUsers | Коллекция строк | Пользовательские ИД в области политики, если явно не исключены, `None` или `All` или или `GuestsOrExternalUsers` . |
| excludeUsers | Коллекция строк | Пользовательские ИД, исключенные из области политики и/или `GuestsOrExternalUsers` . |
| includeGroups | Коллекция строк | Групповые ID в области политики, если явно не исключены, или `All` . |
| excludeGroups | Коллекция строк | Групповые ID исключены из области политики. |
| includeRoles | Коллекция строк | Role IDs in scope of policy unless explicitly excluded, or `All` . |
| excludeRoles | Коллекция строк | ID роли, исключенные из области политики. |

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

