---
title: тип ресурса statusDetails
description: Описывает состояние события подготовка и связанные с ним ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d817c0aa46dde6b49debd849d8fd2ae61e06a672
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956822"
---
# <a name="statusdetails-resource-type"></a>тип ресурса statusDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние события подготовка и связанные с ним ошибки. Он наследуется из [statusBase и](/graph/api/resources/statusbase) используется только при задании состояния `failure` .  

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|statusBase|Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`. Унаследованный от statusBase.|
|additionalDetails|Строка|Дополнительные сведения в случае ошибки.|
|errorCategory|Строка|Классифицировать код ошибки. Возможные значения: `Failure`, `NonServiceFailure`, `Success`.|
|errorCode|String|Уникальный код ошибки, если таковое произошло. [Подробнее](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|reason|Строка|Суммирует состояние и описывает причины, по которым произошел этот статус.|
|recommendedAction|Строка|Обеспечивает разрешение соответствующей ошибки.|

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


