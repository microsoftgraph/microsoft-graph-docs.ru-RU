---
title: тип ресурса conditionalAccessPlatforms
description: Платформы, включенные и исключенные из области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71c8b38b59d30ce1e8e1fa1c7668c41a5d2288c2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945707"
---
# <a name="conditionalaccessplatforms-resource-type"></a>тип ресурса conditionalAccessPlatforms

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Платформы, включенные и исключенные из области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|includePlatforms|коллекция conditionalAccessDevicePlatform| Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.|
|excludePlatforms|коллекция conditionalAccessDevicePlatform| Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPlatforms",
  "baseType": null
}-->

```json
{
  "includePlatforms": ["String"],
  "excludePlatforms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPlatforms resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

