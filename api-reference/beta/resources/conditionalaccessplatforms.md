---
title: Тип ресурса conditionalAccessPlatforms
description: Платформы, включенные в область политики и исключаемые из нее.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3899a47a3a952d6546f308868deefbe2cdd89591
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704298"
---
# <a name="conditionalaccessplatforms-resource-type"></a>Тип ресурса conditionalAccessPlatforms

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Платформы, включенные в область политики и исключаемые из нее.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|includePlatforms|Коллекция conditionalAccessDevicePlatform| Возможные значения: , , , , , , `all``unknownFutureValue, `linux'. `macOS``windowsPhone``windows``iOS``android`|
|excludePlatforms|Коллекция conditionalAccessDevicePlatform| Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`, `linux`.|

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

