---
title: Тип ресурса signInStatus
description: Предоставляет состояние (успешное или неудачное) для этого.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: d7428c2a73d0b4a114599dad8ac1740d91ba5865
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132638"
---
# <a name="signinstatus-resource-type"></a>Тип ресурса signInStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет состояние (успешное или неудачное) для этого.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalDetails|Строка|Предоставляет дополнительные сведения об активности при входе|
|errorCode|Int32|Предоставляет код ошибки из 5–6 цифр, который создается при сбое при входе. Ознакомьтесь [со списком кодов ошибок и сообщений.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)|
|failureReason|String|Предоставляет сообщение об ошибке или причину сбоя для соответствующего действия при входе. Ознакомьтесь [со списком кодов ошибок и сообщений.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)|

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


