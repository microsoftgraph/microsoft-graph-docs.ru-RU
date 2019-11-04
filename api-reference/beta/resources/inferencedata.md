---
title: Тип ресурса Инференцедата
description: Тип ресурса Инференцедата
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 43d6585243eed560a6a8f77268305b7d7f5824a8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938851"
---
# <a name="inferencedata-resource-type"></a>Тип ресурса Инференцедата

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип ресурса [инференцедата](inferencedata.md) предоставляет дополнительные сведения об объекте, который был создан с помощью получения сведений о пользователе. Эти сведения будут представлены, когда данные в определенной сущности появлялись на основе машинного обучения или другого процесса обработки данных.

## <a name="properties"></a>Свойства

| Свойство              | Тип        | Описание                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|конфиденцескоре        |Двойное с плавающей точкой       | Показатель достоверности, отражающий точность данных, выведенных о пользователе.   |
|усерхасверифиедаккураци|Логический      | Записывается, если пользователь подтвердил получение значения true или false.        |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceData",
  "baseType": null
}-->

```json
{
  "confidenceScore": 1024,
  "userHasVerifiedAccuracy": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->