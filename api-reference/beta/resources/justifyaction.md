---
title: Тип ресурса Жустифяктион
description: Указывает, что для указанной операции необходимо обоснование.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bc96062febc15310de6a3b2ed04f96a8cf1e69e5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939315"
---
# <a name="justifyaction-resource-type"></a>Тип ресурса Жустифяктион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, что для указанной операции необходимо обоснование. API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateApplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateClassificationResults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateRemoval.md) могут возвращать **жустифяктион**. Обоснование предоставляется с помощью [лабелингоптионс](../resources/labelingoptions.md). Предыдущий вызов должен повторяться, но свойство **довнградежустификатион** объекта **лабелингоптионс** Set с сообщением обоснования предоставляется с помощью пользовательского ввода или логики приложения.

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