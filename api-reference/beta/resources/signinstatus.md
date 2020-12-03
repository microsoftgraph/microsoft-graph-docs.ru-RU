---
title: Тип ресурса Сигнинстатус
description: Предоставляет состояние входа (успешный или неудачный) входа
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: 5e0b1e3bbca66bd43aa55e0f58739572cdb84c2f
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563620"
---
# <a name="signinstatus-resource-type"></a>Тип ресурса Сигнинстатус

Пространство имен: Microsoft. Graph предоставляет состояние входа (успешную или неудачную) входа



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalDetails|String|Предоставляет дополнительные сведения об активности входа|
|errorCode|Int32|Предоставляет код ошибки 5-6, который создается при сбое входа. Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
|failureReason|String|Содержит сообщение об ошибке или причину сбоя для соответствующего действия при входе. Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|

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


