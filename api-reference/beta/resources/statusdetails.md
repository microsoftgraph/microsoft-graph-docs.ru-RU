---
title: Тип ресурса statusDetails
description: Описывает состояние события предоставления и связанные ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 81ea4a75970e37a360c402aced66f01ccb9e7c47
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292614"
---
# <a name="statusdetails-resource-type"></a>Тип ресурса statusDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние события предоставления и связанные ошибки. Он наследуется от [statusBase и](/graph/api/resources/statusbase) используется только в том случае, если задан статус `failure` .  

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|String|Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`. Наследуется от statusBase.|
|additionalDetails|String|Дополнительные сведения в случае ошибки.|
|errorCategory|String|Классифицировать код ошибки. Возможные значения: `Failure`, `NonServiceFailure`, `Success`.|
|errorCode|String|Уникальный код ошибки, если таковое произошло. [Подробнее](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|reason|String|Суммирует состояние и описывает, почему это состояние произошло.|
|recommendedAction|String|Предоставляет разрешение соответствующей ошибки.|

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


