---
title: Тип ресурса participantInfo
description: Содержит дополнительные свойства сведения об удостоверениях, участников
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7860c80da8e0f56ca425cffe8876d6003fba1d0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991414"
---
# <a name="participantinfo-resource-type"></a>Тип ресурса participantInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит дополнительные свойства сведения об удостоверениях, участников

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание  |
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
