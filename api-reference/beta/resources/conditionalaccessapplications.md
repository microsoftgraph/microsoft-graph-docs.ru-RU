---
title: тип ресурса conditionalAccessApplications
description: Представляет приложения и действия пользователей, включенные и исключенные из области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d688b529e32390c2330cf8cb3558994c3e752a25
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547685"
---
# <a name="conditionalaccessapplications-resource-type"></a>тип ресурса conditionalAccessApplications

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложения и действия пользователей, включенные в политику и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| includeApplications | Коллекция строк | Список ID приложений, к который применяется политика, если явно не исключено (в исключенииApplications). Также можно установить `All` . |
| excludeApplications | Коллекция строк | Список ID приложений явно исключен из политики. |
| includeUserActions | Коллекция строк | Действия пользователя, которые необходимо включить. Поддерживаемые значения `urn:user:registersecurityinfo` и `urn:user:registerdevice` |
| includeAuthenticationContextClassReferences | Коллекция строк | Ссылки на класс контекста проверки подлинности включаются. Поддерживаемые значения `c1` проходят `c25` . |

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

