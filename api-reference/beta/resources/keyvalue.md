---
title: Тип ресурса keyValue
description: Предоставляет дополнительные важные сведения о запросе на вход
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3459f827f35049b383e732c805d61371577b2260
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135396"
---
# <a name="keyvalue-resource-type"></a>Тип ресурса keyValue

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет дополнительные сведения об обработке проверки подлинности, такие как имя сервера и наличие подсказок для входов и домена.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|key|Строка|Содержит имя поля, с которое связано значение. Если в запрос на вход включена подсказка о входе или домене, соответствующие поля включаются в качестве пар "ключ-значение". Возможные ключи: `Login hint present` , `Domain hint present` .|
|value|String|Содержит соответствующее значение для указанного ключа. Значением является, если подсказка для входов была включена в запрос на `true` вход; в противном случае `false` . Значением `true` является, если подсказка домена была включена в запрос на вход; в противном случае `false` .|

## <a name="json-representation"></a>Представление в формате JSON

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


