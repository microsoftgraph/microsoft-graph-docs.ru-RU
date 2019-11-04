---
title: Тип ресурса Довнградежустификатион
description: Представляет ввод пользователя по причине выполнения возврата к предыдущей версии.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aacc32ac86df4eda087f49dbb3dca05a356e8080
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939427"
---
# <a name="downgradejustification-resource-type"></a>Тип ресурса Довнградежустификатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ввод пользователя по причине выполнения возврата к предыдущей версии. Выравнивание на более ранней версии может потребоваться на основе конфигурации политики меток в центре безопасности и соответствия требованиям Office.

## <a name="properties"></a>Свойства

| Свойство             | Тип    | Описание                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| исдовнградежустифиед | Логический | Указывает, является ли переход на предыдущее или не выровненный.                                              |
| жустификатионмессаже | Строка  | Сообщение, указывающее, почему выравниваются более ранние версии. Сообщение будет отображаться в разделе Журналы администрирования. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.downgradeJustification",
  "baseType": null
}-->

```json
{
  "isDowngradeJustified": true,
  "justificationMessage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "downgradeJustification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->