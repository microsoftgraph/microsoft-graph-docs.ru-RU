---
title: signInStatus resource type
description: Предоставляет состояние входного знака (Успешность или сбой) входного знака
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 350ed66245164b5745d7b6f0bc962ebab5b1b4e46e8d7fc6b9a5c45b17ccc3a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54222674"
---
# <a name="signinstatus-resource-type"></a>signInStatus resource type

Пространство имен: microsoft.graph

Предоставляет статус входного знака (Успешность или сбой) входного знака.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalDetails|String|Предоставляет дополнительные сведения о действии для входов|
|errorCode|Int32|Предоставляет код ошибки в 5-6 цифр, созданный во время сбоя при входе. Ознакомьтесь со [списком кодов и сообщений об ошибках.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)|
|failureReason|String|Предоставляет сообщение об ошибке или причину сбоя для соответствующей активности регистрации. Ознакомьтесь со [списком кодов и сообщений об ошибках.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)|

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

