---
title: Тип ресурса Емплойиоргдата
description: Представляет данные организации, связанные с пользователем.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: cmmdesai
ms.openlocfilehash: f8a8ba6add4a68ffa0759346d97cfebbb4199f1c
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635626"
---
# <a name="employeeorgdata-resource-type"></a>Тип ресурса Емплойиоргдата

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные организации, связанные с пользователем. Свойство **емплойиоргдата** объекта [User](user.md) — это коллекция атрибутов Организации.

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
| division | String | Имя подразделения, в котором работает пользователь. <br><br>Возвращается только на `$select`. Поддерживает `$filter`. |
| costCenter | String | Центр затрат, связанный с пользователем. <br><br>Возвращается только на `$select`. Поддерживает `$filter`. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.employeeOrgData"
}-->

```json
{
  "costCenter": "string",
  "division": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-10-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "employeeOrgData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
