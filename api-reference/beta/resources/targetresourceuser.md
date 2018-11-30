---
title: Тип ресурса targetResourceUser
description: Указывает объект пользователя, который был добавлен, обновлении или удалении администраторами с как часть аудита активности. На основе targetResource ресурсов.
ms.openlocfilehash: 632d0551b3aba434c3309c8c874947708eb9a9f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078097"
---
# <a name="targetresourceuser-resource-type"></a>Тип ресурса targetResourceUser
Указывает объект пользователя, который был добавлен, обновлении или удалении администраторами с как часть аудита активности. На основе [targetResource](targetresource.md) ресурсов.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|userPrincipalName|String|Указывает уникальный идентификатор пользователя. Ссылается на идентификатор пользователя для определенного пользователя.|

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