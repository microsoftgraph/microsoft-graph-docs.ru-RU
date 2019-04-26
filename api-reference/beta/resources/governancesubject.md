---
title: Тип ресурса Говернанцесубжект
description: Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).
localization_priority: Normal
ms.openlocfilehash: 5ad4b30abaec66b8ad35835795848645ddd9f17b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333696"
---
# <a name="governancesubject-resource-type"></a>Тип ресурса Говернанцесубжект

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).


## <a name="properties"></a>Свойства
| Свойство  | Тип       |Описание|
|:----------|:----------|:----------|
|id         |Строка     | Идентификатор субъекта.|
|type       |String     |Тип субъекта. Возможные значения: ``User``, ``Group``и. ``ServicePrincipal``|
|displayName|Строка     |Отображаемое имя субъекта.|
|email      |String     |Адрес электронной почты субъекта пользователя. Если тема находится в других типах, она пуста.|
|principalName|String   |Имя субъекта пользователя. Если тема находится в других типах, она пуста.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
