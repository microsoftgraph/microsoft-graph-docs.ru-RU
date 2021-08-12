---
title: тип ресурса employeeOrgData
description: Представляет данные организации, связанные с пользователем.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: cmmdesai
ms.openlocfilehash: e1fbbc82a4b3d9875b5e277c87d59877e162c5555b0bb2d5dcf6b0124d9227af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180868"
---
# <a name="employeeorgdata-resource-type"></a>тип ресурса employeeOrgData

Пространство имен: microsoft.graph

Представляет данные организации, связанные с пользователем. Свойство **employeeOrgData** сущности [пользователя](user.md) — это коллекция атрибутов организации.

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
| division | String | Имя подразделения, в котором работает пользователь. <br><br>Возвращается только с помощью оператора `$select`. Поддерживает `$filter`. |
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
