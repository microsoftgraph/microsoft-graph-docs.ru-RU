---
title: Тип ресурса Инференцедата
description: Тип ресурса Инференцедата
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 412d96d3eb497681e65dacd2f7a0576b4071a9aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016501"
---
# <a name="inferencedata-resource-type"></a>Тип ресурса Инференцедата

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип ресурса [инференцедата](inferencedata.md) предоставляет дополнительные сведения об объекте, который был создан с помощью получения сведений о пользователе. Эти сведения будут представлены, когда данные в определенной сущности появлялись на основе машинного обучения или другого процесса обработки данных.

## <a name="properties"></a>Свойства

| Свойство              | Тип        | Описание                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|конфиденцескоре        |Двойное с плавающей точкой       | Показатель достоверности, отражающий точность данных, выведенных о пользователе.   |
|усерхасверифиедаккураци|Boolean      | Записывается, если пользователь подтвердил получение значения true или false.        |

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

