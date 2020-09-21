---
title: Тип ресурса Говернанцесубжект
description: Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 12f99f7face3013a3286b95ce90c377ff2d1bbf5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989516"
---
# <a name="governancesubject-resource-type"></a>Тип ресурса Говернанцесубжект

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).


## <a name="properties"></a>Свойства
| Свойство  | Тип       |Описание|
|:----------|:----------|:----------|
|id         |String     | Идентификатор субъекта.|
|type       |String     |Тип субъекта. Возможные значения: ``User`` , ``Group`` и ``ServicePrincipal`` .|
|displayName|String     |Отображаемое имя субъекта.|
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


