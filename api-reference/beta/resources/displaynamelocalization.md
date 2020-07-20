---
title: Тип ресурса Дисплайнамелокализатион
description: Предоставляет администратору возможность настраивать строку, используемую в общедоступном интерфейсе Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8ae6c62acfacfccd22cc9985386762a2f61a2bc7
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050860"
---
# <a name="displaynamelocalization-resource-type"></a>Тип ресурса Дисплайнамелокализатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет администратору возможность настраивать строку, используемую в общедоступном интерфейсе Microsoft 365.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName   |String       | Если этот параметр задан, то значение этого поля содержит строку **DisplayName** , заданную для языка, который указан в поле **лангуажетаг** .|
|лангуажетаг   |String       | Предоставляет язык и региональные параметры, а также понятное имя языка, в котором указано поле **DisplayName** .                  |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.displayNameLocalization",
  "baseType": null
}-->

```json
{
  "displayName": "string",
  "languageTag": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "displayNameLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
