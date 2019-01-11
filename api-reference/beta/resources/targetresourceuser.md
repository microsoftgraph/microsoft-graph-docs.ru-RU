---
title: Тип ресурса targetResourceUser
description: Указывает объект пользователя, который был добавлен, обновлении или удалении администраторами с как часть аудита активности. На основе targetResource ресурсов.
localization_priority: Normal
ms.openlocfilehash: 9c71ead1b358b72a1b531abac56018fa71d084e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831930"
---
# <a name="targetresourceuser-resource-type"></a>Тип ресурса targetResourceUser
Указывает объект пользователя, который был добавлен, обновлении или удалении администраторами с как часть аудита активности. На основе [targetResource](targetresource.md) ресурсов.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|userPrincipalName|Строка|Указывает уникальный идентификатор пользователя. Ссылается на идентификатор пользователя для определенного пользователя.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
