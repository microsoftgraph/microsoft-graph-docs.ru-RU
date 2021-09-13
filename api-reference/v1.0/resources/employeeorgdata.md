---
title: тип ресурса employeeOrgData
description: Представляет данные организации, связанные с пользователем.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: cmmdesai
ms.openlocfilehash: 8a0ee00ed1165eddd69a212419292a7690514238
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123610"
---
# <a name="employeeorgdata-resource-type"></a>тип ресурса employeeOrgData

Пространство имен: microsoft.graph

Представляет данные организации, связанные с пользователем. Свойство **employeeOrgData** сущности [пользователя](user.md) — это коллекция атрибутов организации.

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
| division | Строка | Имя подразделения, в котором работает пользователь. <br><br>Возвращается только с помощью оператора `$select`. Поддерживает `$filter`. |
| costCenter | String | Центр затрат, связанный с пользователем. <br><br>Возвращается только с помощью оператора `$select`. Поддерживает `$filter`. |

## <a name="json-representation"></a>Представление JSON

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
