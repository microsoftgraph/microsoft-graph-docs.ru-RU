---
title: тип ресурса provisioningErrorInfo
description: Описывает состояние события подготовка и связанные с ним ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: de8804ab2ae1e1e8f9516e25c0f0a5522d86a0ff2c3722fb9c10e47bc575869c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205200"
---
# <a name="provisioningerrorinfo-resource-type"></a>тип ресурса provisioningErrorInfo

Пространство имен: microsoft.graph


Описывает состояние события подготовка и связанные с ним ошибки. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|additionalDetails|String|Дополнительные сведения в случае ошибки.|
|errorCategory|provisioningStatusErrorCategory|Классифицировать код ошибки. Возможные значения `failure` : `nonServiceFailure` , `success` , `unknownFutureValue`|
|errorCode|String|Уникальный код ошибки, если таковое произошло. [Подробнее](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|reason|String|Суммирует состояние и описывает причины, по которым произошел этот статус.|
|recommendedAction|String|Обеспечивает разрешение соответствующей ошибки.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningErrorInfo",
  "baseType": null
}-->

```json
{
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
  "description": "provisioningErrorInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


