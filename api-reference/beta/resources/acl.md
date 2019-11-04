---
title: Тип ресурса ACL
description: Запись управления доступом для элемента, индексируемого Екстерналконнектион поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0e94f0442f1c2f7f1a1118f07a4e7a86407eee94
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939118"
---
# <a name="acl-resource-type"></a>Тип ресурса ACL

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запись управления доступом для элемента, индексируемого [Екстерналконнектион](externalconnection.md)поиска Microsoft Search.

## <a name="properties"></a>Свойства

| Свойство       | Тип   | Описание                                        |
|:---------------|:-------|:---------------------------------------------------|
| акцесстипе     | Строка | Доступ, назначенный удостоверению. Возможные значения: `grant`, `deny`. |
| идентитисаурце | Строка | Необходимо указать значение `Azure Active Directory`.           |
| type           | String | Тип удостоверения. Возможные значения: `user`, `group`, `everyone`, `everyoneExceptGuests`. |
| value          | String | Идентификатор Azure Active Directory. Если `type` задано `group`значение `value` `user` или, для пользователя или группы задан идентификатор объекта. Если `type` задано `everyoneExceptGuests`значение `value` `everyone` или, в качестве идентификатора клиента для клиента Azure Active Directory. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.acl",
  "baseType": null
}-->

```json
{
  "accessType": "String",
  "identitySource": "String",
  "type": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "acl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
