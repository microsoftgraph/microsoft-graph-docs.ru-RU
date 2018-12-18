---
title: Тип ресурса WorksheetProtectionOptions
description: Представляет параметры защиты листа.
author: lumine2008
ms.openlocfilehash: 772c8b5eca7e9754a6bbc00e43cac102680974a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348575"
---
# <a name="worksheetprotectionoptions-resource-type"></a>Тип ресурса WorksheetProtectionOptions

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет параметры защиты листа.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowAutoFilter|boolean|Представляет параметр защиты листа, разрешающий использовать функцию автофильтра.|
|allowDeleteColumns|boolean|Представляет параметр защиты листа, разрешающий удалять столбцы.|
|allowDeleteRows|boolean|Представляет параметр защиты листа, разрешающий удалять строки.|
|allowFormatCells|boolean|Представляет параметр защиты листа, разрешающий форматировать ячейки.|
|allowFormatColumns|boolean|Представляет параметр защиты листа, разрешающий форматировать столбцы.|
|allowFormatRows|boolean|Представляет параметр защиты листа, разрешающий форматировать строки.|
|allowInsertColumns|boolean|Представляет параметр защиты листа, разрешающий вставлять столбцы.|
|allowInsertHyperlinks|boolean|Представляет параметр защиты листа, разрешающий вставлять гиперссылки.|
|allowInsertRows|boolean|Представляет параметр защиты листа, разрешающий вставлять строки.|
|allowPivotTables|boolean|Представляет параметр защиты листа, разрешающий использовать функцию сводных таблиц.|
|allowSort|boolean|Представляет параметр защиты листа, разрешающий использовать функцию сортировки.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtectionOptions"
}-->

```json
{
  "allowAutoFilter": true,
  "allowDeleteColumns": true,
  "allowDeleteRows": true,
  "allowFormatCells": true,
  "allowFormatColumns": true,
  "allowFormatRows": true,
  "allowInsertColumns": true,
  "allowInsertHyperlinks": true,
  "allowInsertRows": true,
  "allowPivotTables": true,
  "allowSort": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->