---
title: тип ресурса justifyAction
description: Указывает, что для указанной операции требуется обоснование.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1db6a91987fd1345ca6a1503dfbd51e3178e9b89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950319"
---
# <a name="justifyaction-resource-type"></a>тип ресурса justifyAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, что для указанной операции требуется обоснование. The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) API may return **justifyAction**. Обоснование предоставляется с [помощью метокOptions](../resources/labelingoptions.md). Предыдущий вызов должен быть повторен, но с свойством **downgradeJustification** **меткиOptions,** за набором с сообщением об оправдании, предоставляемым с помощью пользовательского ввода или логики приложения.

## <a name="properties"></a>Свойства

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.justifyAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "justifyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

