---
title: Тип ресурса ACL
description: Запись управления доступом для элемента, индексируемого Екстерналконнектион поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6d390ac0fee3063bd8f0d292d14e04b2616c1d00
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193535"
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
| идентитисаурце | String | Источник удостоверения. Возможные значения: `azureActiveDirectory` или `external` .           |
| type           | String | Тип удостоверения. Возможные значения: `user` , `group` ,, `everyone` `everyoneExceptGuests` Если идентитисаурце, `azureActiveDirectory` и только в том `group` случае, если идентитисаурце `external` . |
| value          | String | Уникальный идентификатор удостоверения. В случае удостоверений Azure Active Directory `value` для этого параметра задается идентификатор объекта пользователя, группы или клиента для типов User, Group и Everyone (and еверйониксцептгуестс) соответственно. В случае внешних групп `value` задается идентификатор [екстерналграуп](externalgroup.md).|

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
