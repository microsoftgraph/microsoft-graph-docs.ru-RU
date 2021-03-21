---
title: тип ресурса employeeOrgData
description: Представляет данные организации, связанные с пользователем.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: cmmdesai
ms.openlocfilehash: 841422920ccfe625bd03d8167c13f2a1eba83088
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960434"
---
# <a name="employeeorgdata-resource-type"></a>тип ресурса employeeOrgData

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные организации, связанные с пользователем. Свойство **employeeOrgData** сущности [пользователя](user.md) — это коллекция атрибутов организации.

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
| division | Строка | Имя подразделения, в котором работает пользователь. <br><br>Возвращается только с помощью оператора `$select`. Поддерживает `$filter`. |
| costCenter | Строка | Центр затрат, связанный с пользователем. <br><br>Возвращается только с помощью оператора `$select`. Поддерживает `$filter`. |

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
