---
title: Тип ресурса Статусдетаилс
description: Описывает состояние события подготовки и связанных с ним ошибок.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 16f014ebc3a188644784434a69e13917f05beaae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029024"
---
# <a name="statusdetails-resource-type"></a>Тип ресурса Статусдетаилс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние события подготовки и связанных с ним ошибок. Он наследуется от [статусбасе](/graph/api/resources/statusbase?view=graph-rest-beta) и используется только в том случае, если для параметра Status задано значение "failure".  

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|String|Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`. Наследуется от Статусбасе.|
|additionalDetails|String|Дополнительные сведения в случае ошибки.|
|errorCategory|String|Классификация кода ошибки.|
|errorCode|String|Уникальный код ошибки (при возникновении ошибки).|
|reason|String|Сводка состояния и описание причин возникновения состояния.|
|рекоммендедактион|String|Предоставляет решение для соответствующей ошибки.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "microsoft.graph.statusBase"
}-->

```json
{
  "status": "failure",
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


