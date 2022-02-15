---
title: тип ресурса conditionalAccessPlatforms
description: Платформы, включенные и исключенные из области политики.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5dec75019dc01b4d1ec12b55b66c34f03cb53630
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804103"
---
# <a name="conditionalaccessplatforms-resource-type"></a>тип ресурса conditionalAccessPlatforms

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Платформы, включенные и исключенные из области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|includePlatforms|коллекция conditionalAccessDevicePlatform| Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`, `linux`. Обратите внимание, что для `Prefer: include-unknown-enum-members` получения следующего значения(ы) в этом развиваемом переуме следует использовать загон [запроса](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `linux`. |
|excludePlatforms|коллекция conditionalAccessDevicePlatform| Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`, `linux`. Обратите внимание, что для `Prefer: include-unknown-enum-members` получения следующего значения(ы) в этом развиваемом переуме следует использовать загон [запроса](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `linux`. |

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

