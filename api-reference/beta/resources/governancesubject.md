---
title: Тип ресурса governanceSubject
description: Представляет пользователей, групп и субъектов-служб, управляемых в управления правами Identity (PIM).
ms.openlocfilehash: c2129a0da488d4e7f425d6ef3596a955269e0da8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075437"
---
# <a name="governancesubject-resource-type"></a>Тип ресурса governanceSubject

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет пользователей, групп и субъектов-служб, управляемых в управления правами Identity (PIM).


## <a name="properties"></a>Свойства
| Свойство  | Тип       |Описание|
|:----------|:----------|:----------|
|id         |String     | Идентификатор субъекта.|
|type       |String     |Тип субъекта. Значение может быть ``User``, ``Group``, и ``ServicePrincipal``.|
|displayName|String     |Отображаемое имя субъекта.|
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