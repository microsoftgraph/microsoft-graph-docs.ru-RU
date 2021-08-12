---
title: тип ресурса plannerUserIds
description: Ресурс **plannerUserIds** представляет список ids пользователей, с которые совместно представлен план. Это открытый тип. Если вы используете Microsoft 365 группы, используйте API групп для управления членством в группе, чтобы поделиться планом группы. Вы также можете добавить в эту коллекцию существующих членов группы, хотя для них не требуется доступ к плану, который принадлежит группе.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b40b1681728bcebe85bab43254bb8414886ff3425d296596364992db7d5c8e7e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223251"
---
# <a name="planneruserids-resource-type"></a>тип ресурса plannerUserIds

Пространство имен: microsoft.graph

Ресурс **plannerUserIds** представляет список ids пользователей, [с](plannerplan.md) которые совместно представлен план. Это открытый тип. Если вы используете Microsoft 365 группы, используйте API групп для управления членством в группе, чтобы поделиться [планом](group.md) группы. Вы также можете добавить в эту коллекцию существующих членов группы, хотя для них не требуется доступ к плану, который принадлежит группе.


## <a name="properties"></a>Свойства
Свойства открытого типа могут быть определены клиентом. В этом случае клиент должен предоставить пользовательские ids в качестве свойств, а их значения — `true` boolean. Когда пользовательские ids больше не являются общими, свойства автоматически удаляются, задав их значения `false` в boolean.


## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

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

### <a name="example"></a>Пример
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

