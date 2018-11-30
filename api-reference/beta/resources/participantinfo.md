---
title: Тип ресурса participantInfo
description: Содержит дополнительные свойства сведения об удостоверениях, участников
ms.openlocfilehash: c6f429e353d80ea53c5f5c00ca084ae7a8a4a7c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074891"
---
# <a name="participantinfo-resource-type"></a>Тип ресурса participantInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит дополнительные свойства сведения об удостоверениях, участников

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Description  |
|:---------------|:------------------------------|:-------------|
| identity       | [identitySet](identityset.md) | [IdentitySet](identityset.md) , связанный с данным участником. |
| languageId     | String                        | Строка языка и региональных параметров языка. |
| область         | String                        | Область участника. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->