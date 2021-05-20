---
title: тип ресурса statusDetails
description: Описывает состояние события подготовка и связанные с ним ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e3333ac030ec08722ad6bcaa58a153fc961469cf
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546909"
---
# <a name="statusdetails-resource-type-deprecated"></a>тип ресурса statusDetails (неподготовленный)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION] 
> API statusDetails обесценена и прекратит возвращать данные om 31 декабря 2021 г. Используйте новый [тип provisioningStatusInfo.](provisioningstatusinfo.md)

Описывает состояние события подготовка и связанные с ним ошибки. Он наследуется из [statusBase и](/graph/api/resources/statusbase) используется только при задании состояния `failure` .  

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|statusBase|Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`. Унаследованный от statusBase.|
|additionalDetails|String|Дополнительные сведения в случае ошибки.|
|errorCategory|String|Классифицировать код ошибки. Возможные значения: `Failure`, `NonServiceFailure`, `Success`.|
|errorCode|String|Уникальный код ошибки, если таковое произошло. [Подробнее](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|reason|String|Суммирует состояние и описывает причины, по которым произошел этот статус.|
|recommendedAction|String|Обеспечивает разрешение соответствующей ошибки.|

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


