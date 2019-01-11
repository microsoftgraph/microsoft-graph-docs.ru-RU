---
title: Тип ресурса governanceSubject
description: Представляет пользователей, групп и субъектов-служб, управляемых в управления правами Identity (PIM).
localization_priority: Normal
ms.openlocfilehash: f3f8762c9136a3ae92269f6c06f52000fb73f710
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832594"
---
# <a name="governancesubject-resource-type"></a>Тип ресурса governanceSubject

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет пользователей, групп и субъектов-служб, управляемых в управления правами Identity (PIM).


## <a name="properties"></a>Свойства
| Свойство  | Тип       |Описание|
|:----------|:----------|:----------|
|id         |Строка     | Идентификатор субъекта.|
|type       |Строка     |Тип субъекта. Значение может быть ``User``, ``Group``, и ``ServicePrincipal``.|
|displayName|Строка     |Отображаемое имя субъекта.|
|email      |String     |Адрес электронной почты субъекта пользователя. Если темы в других типах, он будет пустым.|
|principalName|String   |Имя субъекта пользователя. Если темы в других типах, он будет пустым.|

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
