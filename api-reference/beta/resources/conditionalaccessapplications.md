---
title: Тип ресурса Кондитионалакцессаппликатионс
description: Представляет приложения и действия пользователя, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba904fec35830bef6cc5a74daa1c4938bd99d250
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269912"
---
# <a name="conditionalaccessapplications-resource-type"></a>Тип ресурса Кондитионалакцессаппликатионс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложения и действия пользователя, включенные в политику и исключенные из нее.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| инклудеаппликатионс | Коллекция строк | Список идентификаторов приложений, к которым применяется политика, если явно не исключено (в Ексклудеаппликатионс). Также можно задать значение `All` . |
| ексклудеаппликатионс | Коллекция строк | Список идентификаторов приложений, явно исключенных из политики. |
| инклудеусерактионс | Коллекция строк | Включаемые действия пользователя. Поддерживаемые значения: `urn:user:registersecurityinfo` и `urn:user:registerdevice` |

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

