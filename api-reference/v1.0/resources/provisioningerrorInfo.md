---
title: тип ресурса provisioningErrorInfo
description: Описывает состояние события подготовка и связанные с ним ошибки.
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f0b6e42fc184db1d8c2044d56820d0e19e89f8c3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019169"
---
# <a name="provisioningerrorinfo-resource-type"></a>тип ресурса provisioningErrorInfo

Пространство имен: microsoft.graph


Описывает состояние события подготовка и связанные с ним ошибки. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|additionalDetails|Строка|Дополнительные сведения в случае ошибки.|
|errorCategory|provisioningStatusErrorCategory|Классифицировать код ошибки. Возможные значения `failure` : `nonServiceFailure` , `success` , `unknownFutureValue`|
|errorCode|String|Уникальный код ошибки, если таковое произошло. [Подробнее](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|reason|Строка|Суммирует состояние и описывает причины, по которым произошел этот статус.|
|recommendedAction|Строка|Обеспечивает разрешение соответствующей ошибки.|

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


