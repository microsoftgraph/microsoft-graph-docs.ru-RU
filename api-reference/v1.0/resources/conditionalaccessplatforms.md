---
title: тип ресурса conditionalAccessPlatforms
description: Платформы, включенные и исключенные из области политики.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ca34f949e910907910a2aa14e64951538ab4bb13
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672541"
---
# <a name="conditionalaccessplatforms-resource-type"></a>тип ресурса conditionalAccessPlatforms

Пространство имен: microsoft.graph

Платформы, включенные и исключенные из области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|includePlatforms|коллекция conditionalAccessDevicePlatform| Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `linux`, `all`, `unknownFutureValue`.|
|excludePlatforms|коллекция conditionalAccessDevicePlatform| Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `linux`, `all`, `unknownFutureValue`.|

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

