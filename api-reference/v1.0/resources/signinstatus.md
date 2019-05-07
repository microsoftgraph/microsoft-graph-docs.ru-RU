---
title: Тип ресурса Сигнинстатус
description: Предоставляет состояние входа (успешный или неудачный) входа
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a57e5bb0e53f5deec4d0c6d92541f7d2bd4744d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629224"
---
# <a name="signinstatus-resource-type"></a>Тип ресурса Сигнинстатус

Предоставляет состояние входа (успешный или неудачный) входа.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalDetails|String|Предоставляет дополнительные сведения об активности входа|
|errorCode|Int32|Предоставляет код ошибки 5 6digit, который создается при сбое входа. Ознакомьтесь со [списком кодов и сообщений об ошибках](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
|failureReason|String|Содержит сообщение об ошибке или причину сбоя для соответствующего действия при входе. Ознакомьтесь со [списком кодов и сообщений об ошибках](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|

## <a name="json-representation"></a>Представление в формате JSON

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
