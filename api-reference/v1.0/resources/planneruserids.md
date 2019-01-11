---
title: Тип ресурса plannerUserIds
description: Ресурс **plannerUserIds** представляет список идентификаторов пользователей, которым предоставлен доступ к плану. Это открытый тип. Если вы используете функцию "Группы Office 365", то для предоставления доступа к плану группы применяйте API для групп (чтобы управлять членством в группах). Вы также можете добавить существующих участников группы в эту коллекцию, хотя им необязательно иметь доступ к плану, принадлежащему группе.
localization_priority: Normal
ms.openlocfilehash: d1ded78b76b2e8284a7563ad43b2c466cda4cc5e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879025"
---
# <a name="planneruserids-resource-type"></a>Тип ресурса plannerUserIds

Ресурс **plannerUserIds** представляет список идентификаторов пользователей, которым предоставлен доступ к [плану](plannerplan.md). Это открытый тип. Если вы используете функцию "Группы Office 365", то для предоставления доступа к плану [группы](group.md) применяйте API для групп (чтобы управлять членством в группах). Вы также можете добавить существующих участников группы в эту коллекцию, хотя им необязательно иметь доступ к плану, принадлежащему группе.


## <a name="properties"></a>Свойства
Клиент может определять свойства открытого типа. В этом случае клиент должен предоставить идентификаторы пользователей в качестве свойств, причем они должны иметь значение `true` (логическое). Если больше не нужно предоставлять доступ для идентификаторов пользователей, задайте для свойств значение `false` (логическое), и свойства будут автоматически удалены.


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

Пример:
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
