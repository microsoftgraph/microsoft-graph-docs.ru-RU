---
title: Тип ресурса signInStatus
description: Предоставляет входа в состояние (успешное или неудачное) входа в программу
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878640"
---
# <a name="signinstatus-resource-type"></a>Тип ресурса signInStatus
Предоставляет входа в состояние (успешное или неудачное) входа в программу



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalDetails|Строка|Дополнительные сведения для входа в действия|
|errorCode|Int32|Содержит код ошибки 5 6digit, созданного во время сбоя входа. Извлечение [списка кодов ошибок и сообщений](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
|failureReason|String|Содержит сообщение об ошибке или причину сбоя для соответствующей операции регистрации. Извлечение [списка кодов ошибок и сообщений](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
