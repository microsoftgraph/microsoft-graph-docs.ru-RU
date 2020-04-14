---
title: Тип ресурса Кондитионалакцессусерс
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 99fa682b787a164896cb638060798cddee07b255
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467938"
---
# <a name="conditionalaccessusers-resource-type"></a>Тип ресурса Кондитионалакцессусерс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| инклудеусерс | Коллекция String | Идентификаторы пользователей в области применения политики, если явно не `None` исключены, `All` или или `GuestsOrExternalUsers`. |
| ексклудеусерс | Коллекция String | Идентификаторы пользователей, исключенные из области применения политики `GuestsOrExternalUsers`и/или. |
| инклудеграупс | Коллекция String | Идентификаторы групп в области политики, если явно не исключены, или `All`. |
| ексклудеграупс | Коллекция String | Идентификаторы групп, исключенные из области применения политики. |
| инклудеролес | Коллекция String | Идентификаторы ролей в области применения политики, если они явно `All`не исключены, или. |
| ексклудеролес | Коллекция String | Идентификаторы ролей, исключенные из области применения политики. |

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