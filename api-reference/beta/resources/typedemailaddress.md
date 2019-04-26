---
title: Тип ресурса Типедемаиладдресс
description: Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты контакта.
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576460"
---
# <a name="typedemailaddress-resource-type"></a>Тип ресурса Типедемаиладдресс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты [контакта](contact.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|String|Адрес электронной почты контакта.|
|name|Строка|Отображаемое имя контакта.|
|type |String |Тип адреса электронной почты. Возможные значения: `unknown`, `work`, `personal`, `main`, `other`. Значение по умолчанию `unknown`—, то есть **адрес** не был задан как определенный тип. |
|Осерлабел |String  |Чтобы указать настраиваемый тип адреса электронной почты, задайте **** для `other`параметра Тип значение и назначьте **осерлабел** настраиваемой строке. Например, вы можете использовать конкретный адрес электронной почты для своих мероприятий. Задайте **** для `other`параметра Type значение, а для параметра **осерлабел** — настраиваемую `Volunteer work`строку (например,). |

## <a name="json-representation"></a>Описание в формате JSON

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
