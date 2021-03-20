---
title: тип ресурса downgradeJustification
description: Представляет пользовательские сведения о том, почему было выполнено понижение.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: bc7336469f93de9e6d2b07fe73df9dce2eafd47f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941801"
---
# <a name="downgradejustification-resource-type"></a>тип ресурса downgradeJustification

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательские сведения о том, почему было выполнено понижение. Обоснование понижения может потребоваться на основе конфигурации политики меток в Центре безопасности и соответствия требованиям Office.

## <a name="properties"></a>Свойства

| Свойство             | Тип    | Описание                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| isDowngradeJustified | Boolean | Указывает, является ли понижение или не оправдано.                                              |
| justificationMessage | Строка  | Сообщение, которое указывает, почему понижение является оправданным. Сообщение будет отображаться в административных журналах. |

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

