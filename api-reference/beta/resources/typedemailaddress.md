---
title: Тип ресурса typedEmailAddress
description: Представляет имя, адреса электронной почты и соответствующий тип адреса электронной почты контакта.
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510710"
---
# <a name="typedemailaddress-resource-type"></a>Тип ресурса typedEmailAddress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет имя, адреса электронной почты и их соответствующий тип адреса электронной почты [контакта](contact.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|String|Адрес электронной почты контакта.|
|name|String|Отображаемое имя контакта.|
|type |Строка |Тип адреса электронной почты. Возможные значения: `unknown`, `work`, `personal`, `main`, `other`. Значение по умолчанию — `unknown`, который означает, что **адрес** не был установлен как определенного типа. |
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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
