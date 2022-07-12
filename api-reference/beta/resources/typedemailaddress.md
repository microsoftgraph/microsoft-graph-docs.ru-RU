---
title: Тип ресурса typedEmailAddress
description: Представляет имя, адреса электронной почты и соответствующий тип адреса электронной почты контакта.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: kevinbellinger
ms.openlocfilehash: 849e566919b22ddaa9c12a275f19139701bf467d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66723495"
---
# <a name="typedemailaddress-resource-type"></a>Тип ресурса typedEmailAddress

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет имя, адреса электронной почты и соответствующий тип адреса электронной почты [контакта](contact.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|String|Адрес электронной почты контакта.|
|name|String|Отображаемое имя контакта.|
|type |String |Тип адреса электронной почты. Возможные значения: `unknown`, `work`, `personal`, `main`, `other`. Значение по умолчанию — `unknown`это означает, **что адрес** не был задан как конкретный тип. |
|otherLabel |String  |Чтобы указать пользовательский тип адреса электронной почты, `other`задайте тип и назначьте **otherLabel** настраиваемой строке. Например, вы можете использовать определенный адрес электронной почты для своих действий во время работы с доброволителями. **Задайте** тип в `other`значение **otherLabel** и задайте настраиваемую строку, например `Volunteer work`. |

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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


