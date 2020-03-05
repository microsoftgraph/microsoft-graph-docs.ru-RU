---
title: Тип ресурса Кондитионалакцессусерс
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 269fe0552c69773fa62b97cf9803b3e0127f655b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507508"
---
# <a name="conditionalaccessusers-resource-type"></a>Тип ресурса Кондитионалакцессусерс

Пространство имен: Microsoft. Graph

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