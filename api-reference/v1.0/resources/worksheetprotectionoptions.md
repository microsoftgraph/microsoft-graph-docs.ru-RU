---
title: Тип ресурса WorksheetProtectionOptions
description: Представляет параметры защиты листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 727d05b1819299f938c21f71e859d06e2455ebb25819bbd96c78dec746cbd753
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182345"
---
# <a name="worksheetprotectionoptions-resource-type"></a>Тип ресурса WorksheetProtectionOptions

Пространство имен: microsoft.graph

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
  "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions"
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

