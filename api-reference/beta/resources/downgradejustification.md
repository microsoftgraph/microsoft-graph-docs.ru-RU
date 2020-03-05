---
title: Тип ресурса Довнградежустификатион
description: Представляет ввод пользователя по причине выполнения возврата к предыдущей версии.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91bcb5a8e12a159bf2c6586a0e3dc49a540a69f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505793"
---
# <a name="downgradejustification-resource-type"></a>Тип ресурса Довнградежустификатион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ввод пользователя по причине выполнения возврата к предыдущей версии. Выравнивание на более ранней версии может потребоваться на основе конфигурации политики меток в центре безопасности и соответствия требованиям Office.

## <a name="properties"></a>Свойства

| Свойство             | Тип    | Описание                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| исдовнградежустифиед | Логический | Указывает, является ли переход на предыдущее или не выровненный.                                              |
| жустификатионмессаже | String  | Сообщение, указывающее, почему выравниваются более ранние версии. Сообщение будет отображаться в разделе Журналы администрирования. |

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