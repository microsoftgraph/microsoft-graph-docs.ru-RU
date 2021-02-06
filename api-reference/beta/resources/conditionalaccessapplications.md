---
title: Тип ресурса conditionalAccessApplications
description: Представляет приложения и действия пользователей, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0a787a1c22209b502e4eed68790629e2e6e1b03b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137403"
---
# <a name="conditionalaccessapplications-resource-type"></a>Тип ресурса conditionalAccessApplications

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложения и действия пользователей, включенные в политику и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| includeApplications | Коллекция объектов string | Список ИД приложений, к которых применяется политика, за исключением явно исключенных (в excludeApplications). Также может быть установлено в `All` . |
| excludeApplications | Коллекция объектов string | Список ИД приложений, явно исключенных из политики. |
| includeUserActions | Коллекция объектов string | Действия пользователей, которые необходимо включить. Поддерживаемые `urn:user:registersecurityinfo` значения: `urn:user:registerdevice` |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

