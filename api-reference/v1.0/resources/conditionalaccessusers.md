---
title: тип ресурса conditionalAccessUsers
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f9930d1d1ac1b5d355699b893bfbf59f047162d1d0c0f39d0303a98b889ab7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229306"
---
# <a name="conditionalaccessusers-resource-type"></a>тип ресурса conditionalAccessUsers

Пространство имен: microsoft.graph

Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeUsers | Коллекция строк | Пользовательские ИД в области политики, если явно не исключены, `None` или `All` или или `GuestsOrExternalUsers` . |
| excludeUsers | Коллекция String | Пользовательские ИД, исключенные из области политики и/или `GuestsOrExternalUsers` . |
| includeGroups | Коллекция String | Групповые ID в области политики, если явно не исключены, или `All` . |
| excludeGroups | Коллекция строк | Групповые ID исключены из области политики. |
| includeRoles | Коллекция String | Role IDs in scope of policy unless explicitly excluded, or `All` . |
| excludeRoles | Коллекция String | ID роли, исключенные из области политики. |

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

