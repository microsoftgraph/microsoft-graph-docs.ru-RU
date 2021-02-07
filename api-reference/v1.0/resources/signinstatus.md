---
title: Тип ресурса signInStatus
description: Предоставляет состояние (успешное или неудачное) для этого.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 37eb91434fd7a5fb0dc65f5c7203effd42f3878e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137090"
---
# <a name="signinstatus-resource-type"></a>Тип ресурса signInStatus

Пространство имен: microsoft.graph

Предоставляет состояние (успешное или неудачное) для этого.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalDetails|String|Предоставляет дополнительные сведения об активности при входе|
|errorCode|Int32|Предоставляет код ошибки из 5–6 цифр, который создается во время сбоя при входе. Ознакомьтесь [со списком кодов ошибок и сообщений.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)|
|failureReason|String|Предоставляет сообщение об ошибке или причину сбоя для соответствующего действия при входе. Ознакомьтесь [со списком кодов ошибок и сообщений.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)|

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

