---
title: Тип ресурса governanceSubject
description: Представляет пользователей, группы и субъекты-службы, управляемые в управление привилегированными пользователями (PIM).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: f898c844a9bf2d461cf73e02abf1852e012c1825
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397574"
---
# <a name="governancesubject-resource-type"></a>Тип ресурса governanceSubject

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей, группы и субъекты-службы, управляемые в управление привилегированными пользователями (PIM).


## <a name="properties"></a>Свойства
| Свойство  | Тип       |Описание|
|:----------|:----------|:----------|
|id         |String     | Идентификатор субъекта.|
|type       |String     |Тип темы. Значение может быть ``User``, ``Group``и ``ServicePrincipal``.|
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


