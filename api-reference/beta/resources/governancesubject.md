---
title: тип ресурсов governanceSubject
description: Представляет пользователей, групп и директоров служб, управляемых в управление привилегированными пользователями (PIM).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 99e668cc18ff38f8a4b26c11d514beddcc020e00
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509639"
---
# <a name="governancesubject-resource-type"></a>тип ресурсов governanceSubject

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей, групп и директоров служб, управляемых в управление привилегированными пользователями (PIM).


## <a name="properties"></a>Свойства
| Свойство  | Тип       |Описание|
|:----------|:----------|:----------|
|id         |Строка     | ID субъекта.|
|type       |Строка     |Тип субъекта. Значение может быть ``User``, ``Group``и ``ServicePrincipal``.|
|displayName|Строка     |Отображение имени субъекта.|
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


