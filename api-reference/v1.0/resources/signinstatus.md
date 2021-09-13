---
title: signInStatus resource type
description: Предоставляет состояние входного знака (Успешность или сбой) входного знака
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 87181dd2ec911d2ebaa613dd4bc7ad4d46182a2d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139585"
---
# <a name="signinstatus-resource-type"></a>signInStatus resource type

Пространство имен: microsoft.graph

Предоставляет статус входного знака (Успешность или сбой) входного знака.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalDetails|Строка|Предоставляет дополнительные сведения о действии для входов|
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

