---
title: Тип ресурса Сигнинстатус
description: Предоставляет состояние входа (успешный или неУдачный) входа
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583573"
---
# <a name="signinstatus-resource-type"></a>Тип ресурса Сигнинстатус
Предоставляет состояние входа (успешный или неУдачный) входа



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalDetails|String|Предоставляет дополнительные сведения об активности входа|
|errorCode|Int32|Предоставляет код ошибки 5 6digit, который создается при сбое входа. Ознакомьтесь со [списком кодов и сообщений об ошибках](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
|failureReason|String|Содержит сообщение об ошибке или причину сбоя для соответствующего действия при входе. Ознакомьтесь со [списком кодов и сообщений об ошибках](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|

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
