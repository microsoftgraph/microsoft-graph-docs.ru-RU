---
title: Тип ресурса typedEmailAddress
description: Представляет имя, адреса электронной почты и соответствующий тип адреса электронной почты контакта.
ms.openlocfilehash: 3f40add32fbc219606b6d78041552fc108803d1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082741"
---
# <a name="typedemailaddress-resource-type"></a>Тип ресурса typedEmailAddress

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет имя, адреса электронной почты и их соответствующий тип адреса электронной почты [контакта](contact.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|String|Адрес электронной почты контакта.|
|name|String|Отображаемое имя контакта.|
|type |String |Тип адреса электронной почты. Возможные значения: `unknown`, `work`, `personal`, `main`, `other`. Значение по умолчанию — `unknown`, который означает, что **адрес** не был установлен как определенного типа. |
|otherLabel |String  |Чтобы сделать настраиваемого типа адреса электронной почты, задать **Тип** `other`и назначьте **otherLabel** настраиваемой строки. Например может использовать действительный адрес электронной почты конкретного авторам действий. Значение **типа** `other`и установите **otherLabel** в настраиваемой строке таких как `Volunteer work`. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
