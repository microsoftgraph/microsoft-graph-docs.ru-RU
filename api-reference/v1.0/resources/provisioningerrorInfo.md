---
title: предоставление типа ресурса «ЭррорИнфо»
description: Описывает состояние события подготовки и связанные с ним ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a682e176b40d58e2dc0a794b58b8561f8948d5a5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547157"
---
# <a name="provisioningerrorinfo-resource-type"></a>предоставление типа ресурса «ЭррорИнфо»

Пространство имен: microsoft.graph


Описывает состояние события подготовки и связанные с ним ошибки. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|additionalDetails|String|Дополнительные сведения в случае ошибки.|
|ошибкаКатегория|положениеСтатусЭррорКатегория|Классифицирует код ошибки. Возможные `failure` значения, `nonServiceFailure` `success` , `unknownFutureValue`|
|errorCode|String|Уникальный код ошибки, если таковые имели место. [Подробнее](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|reason|String|Суммирует статус и описывает, почему статус произошел.|
|рекомендуемая Действий|String|Предоставляет разрешение для соответствующей ошибки.|

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


