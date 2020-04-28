---
title: Тип ресурса Говернанцесубжект
description: Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4d1fbf75b4e9643dc0e3b968ace7a013616904ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497173"
---
# <a name="governancesubject-resource-type"></a>Тип ресурса Говернанцесубжект

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).


## <a name="properties"></a>Свойства
| Свойство  | Тип       |Описание|
|:----------|:----------|:----------|
|id         |String     | Идентификатор субъекта.|
|type       |String     |Тип субъекта. Возможные значения: ``User``, ``Group``и. ``ServicePrincipal``|
|displayName|Строка     |Отображаемое имя субъекта.|
|email      |String     |Адрес электронной почты субъекта пользователя. Если тема находится в других типах, она пуста.|
|principalName|String   |Имя субъекта пользователя. Если тема находится в других типах, она пуста.|

## <a name="relationships"></a>Связи
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
