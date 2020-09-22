---
title: Тип ресурса ACL
description: Запись управления доступом для элемента, индексируемого Екстерналконнектион поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d0745ab4a04233a654b829da8f93defb855fc0f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024558"
---
# <a name="acl-resource-type"></a>Тип ресурса ACL

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запись управления доступом для элемента, индексируемого [Екстерналконнектион](externalconnection.md)поиска Microsoft Search.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство       | Тип   | Описание                                        |
|:---------------|:-------|:---------------------------------------------------|
| акцесстипе     | String | Доступ, назначенный удостоверению. Возможные значения: `grant`, `deny`. |
| идентитисаурце | String | Необходимо указать значение `Azure Active Directory`.           |
| type           | String | Тип удостоверения. Возможные значения: `user`, `group`, `everyone`, `everyoneExceptGuests`. |
| value          | String | Идентификатор Azure Active Directory. Если задано значение `type` `user` или `group` , `value` для пользователя или группы задан идентификатор объекта. Если задано значение `type` `everyone` или `everyoneExceptGuests` , `value` в качестве идентификатора клиента для клиента Azure Active Directory. |

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


