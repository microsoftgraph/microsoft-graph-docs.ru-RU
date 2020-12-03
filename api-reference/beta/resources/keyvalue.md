---
title: Тип ресурса Ключзначение
description: Предоставляет дополнительные релевантные сведения о запросе на вход
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78dd4f6ede6e918bb1caaae3761ef258b4e0a427
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524703"
---
# <a name="keyvalue-resource-type"></a>Тип ресурса Ключзначение

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет дополнительные сведения об обработке проверки подлинности, такие как имя сервера и наличие подсказок для входа и домена.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|key|String|Содержит имя поля, с которым связано значение. Если подсказка входа или домена включена в запрос на вход, соответствующие поля включаются в качестве пар "ключ-значение". Возможные ключи: `Login hint present` , `Domain hint present` .|
|value|String|Содержит соответствующее значение для указанного ключа. Значение, `true` Если подсказка для входа была включена в запрос на вход; в противном случае `false` . Значение, `true` Если подсказка домена включена в запрос на вход; в противном случае `false` .|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue",
  "baseType": null
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


