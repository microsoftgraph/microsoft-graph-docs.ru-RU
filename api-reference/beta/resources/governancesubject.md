---
title: тип ресурсов governanceSubject
description: Представляет пользователей, групп и директоров служб, управляемых в управление привилегированными пользователями (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: c3e37d9391bedba160c67f6c30e2f386a1524a9f
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454236"
---
# <a name="governancesubject-resource-type"></a>тип ресурсов governanceSubject

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей, групп и директоров служб, управляемых в управление привилегированными пользователями (PIM).


## <a name="properties"></a>Свойства
| Свойство  | Тип       |Описание|
|:----------|:----------|:----------|
|id         |String     | ID субъекта.|
|type       |String     |Тип субъекта. Значение может быть ``User`` , ``Group`` и ``ServicePrincipal`` .|
|displayName|String     |Отображение имени субъекта.|
|email      |String     |Адрес электронной почты субъекта пользователя. Если объект находится в других типах, он пуст.|
|principalName|String   |Основное имя субъекта пользователя. Если объект находится в других типах, он пуст.|

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


