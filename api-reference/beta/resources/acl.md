---
title: Тип ресурса ACL
description: Запись управления доступом для элемента, индексируемого Екстерналконнектион поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a26004cf20a5f8c5c032eeade8f657fdf8bd93c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703942"
---
# <a name="acl-resource-type"></a>Тип ресурса ACL

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запись управления доступом для элемента, индексируемого [Екстерналконнектион](externalconnection.md)поиска Microsoft Search.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство       | Тип   | Описание                                        |
|:---------------|:-------|:---------------------------------------------------|
| акцесстипе     | String | Доступ, назначенный удостоверению. Возможные значения: `grant`, `deny`. |
| идентитисаурце | String | Необходимо указать значение `Azure Active Directory`.           |
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
