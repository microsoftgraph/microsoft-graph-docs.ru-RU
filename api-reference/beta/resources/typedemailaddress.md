---
title: Тип ресурса Типедемаиладдресс
description: Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты контакта.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 6641d05542fb6d6e376343dff98508183f5a012b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812767"
---
# <a name="typedemailaddress-resource-type"></a>Тип ресурса Типедемаиладдресс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты [контакта](contact.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|String|Адрес электронной почты контакта.|
|name|String|Отображаемое имя контакта.|
|type |String |Тип адреса электронной почты. Возможные значения: `unknown`, `work`, `personal`, `main`, `other`. Значение по умолчанию —, то есть `unknown` **адрес** не был задан как определенный тип. |
|осерлабел |String  |Чтобы указать настраиваемый тип адреса электронной почты, задайте для параметра **тип** значение `other` и назначьте **осерлабел** настраиваемой строке. Например, вы можете использовать конкретный адрес электронной почты для своих мероприятий. Задайте для параметра **Type** значение `other` , а для параметра **осерлабел** — настраиваемую строку (например,) `Volunteer work` . |

## <a name="json-representation"></a>Представление в формате JSON

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
