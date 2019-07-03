---
title: Тип ресурса Статусдетаилс
description: Описывает состояние события подготовки и связанных с ним ошибок.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 88880fbe88c0bd702eefeac5bed9668aac12a356
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455184"
---
# <a name="statusdetails-resource-type"></a>Тип ресурса Статусдетаилс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние события подготовки и связанных с ним ошибок. Он наследуется от [статусбасе](/graph/api/resources/statusbase?view=graph-rest-beta) и используется только в том случае, если для параметра Status задано значение "failure".  

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|String|Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`. Наследуется от Статусбасе.|
|additionalDetails|String|Дополнительные сведения в случае ошибки.|
|errorCategory|String|Классификация кода ошибки.|
|errorCode|String|Уникальный код ошибки (при возникновении ошибки).|
|причиной|String|Сводка состояния и описание причин возникновения состояния.|
|Рекоммендедактион|String|Предоставляет решение для соответствующей ошибки.|

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
