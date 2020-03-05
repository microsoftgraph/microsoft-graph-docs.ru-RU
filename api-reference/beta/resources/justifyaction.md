---
title: Тип ресурса Жустифяктион
description: Указывает, что для указанной операции необходимо обоснование.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6f2246ad9d166bc51dae79032c95fc3b2d55b72e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523039"
---
# <a name="justifyaction-resource-type"></a>Тип ресурса Жустифяктион

Пространство имен: Microsoft. Graph

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