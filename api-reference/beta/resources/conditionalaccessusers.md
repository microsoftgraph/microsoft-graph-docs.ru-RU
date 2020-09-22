---
title: Тип ресурса Кондитионалакцессусерс
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d1294551fd568b9f41072d3707d64a88d4b04edc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994241"
---
# <a name="conditionalaccessusers-resource-type"></a>Тип ресурса Кондитионалакцессусерс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| инклудеусерс | Коллекция String | Идентификаторы пользователей в области применения политики, если явно не исключены, или или `None` `All` `GuestsOrExternalUsers` . |
| ексклудеусерс | Коллекция String | Идентификаторы пользователей, исключенные из области применения политики и/или `GuestsOrExternalUsers` . |
| инклудеграупс | Коллекция String | Идентификаторы групп в области политики, если явно не исключены, или `All` . |
| ексклудеграупс | Коллекция String | Идентификаторы групп, исключенные из области применения политики. |
| инклудеролес | Коллекция String | Идентификаторы ролей в области применения политики, если они явно не исключены, или `All` . |
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

