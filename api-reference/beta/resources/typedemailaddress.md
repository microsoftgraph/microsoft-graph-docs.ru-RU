---
title: Тип ресурса Типедемаиладдресс
description: Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты контакта.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7d6c064e7a87b0e9c776a5691f24b48dfff56422
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519633"
---
# <a name="typedemailaddress-resource-type"></a>Тип ресурса Типедемаиладдресс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты [контакта](contact.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|String|Адрес электронной почты контакта.|
|name|Строка|Отображаемое имя контакта.|
|type |String |Тип адреса электронной почты. Возможные значения: `unknown`, `work`, `personal`, `main`, `other`. Значение по умолчанию `unknown`—, то есть **адрес** не был задан как определенный тип. |
|осерлабел |String  |Чтобы указать настраиваемый тип адреса электронной почты, задайте **type** для `other`параметра Тип значение и назначьте **осерлабел** настраиваемой строке. Например, вы можете использовать конкретный адрес электронной почты для своих мероприятий. Задайте **type** для `other`параметра Type значение, а для параметра **осерлабел** — настраиваемую `Volunteer work`строку (например,). |

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
