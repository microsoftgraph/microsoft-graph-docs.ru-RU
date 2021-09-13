---
title: тип ресурса conditionalAccessUsers
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0b4c3298f233fbd47838b9eeaf12230445c0f6cc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084582"
---
# <a name="conditionalaccessusers-resource-type"></a>тип ресурса conditionalAccessUsers

Пространство имен: microsoft.graph

Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeUsers | Коллекция String | Пользовательские ИД в области политики, если явно не исключены, `None` или `All` или или `GuestsOrExternalUsers` . |
| excludeUsers | Коллекция String | Пользовательские ИД, исключенные из области политики и/или `GuestsOrExternalUsers` . |
| includeGroups | Коллекция String | Групповые ID в области политики, если явно не исключены, или `All` . |
| excludeGroups | Коллекция String | Групповые ID исключены из области политики. |
| includeRoles | Коллекция String | Role IDs in scope of policy unless explicitly excluded, or `All` . |
| excludeRoles | Коллекция String | ID роли, исключенные из области политики. |

## <a name="relationships"></a>Отношения

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

