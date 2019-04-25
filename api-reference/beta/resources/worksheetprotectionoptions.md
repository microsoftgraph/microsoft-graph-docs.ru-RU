---
title: Тип ресурса WorksheetProtectionOptions
description: Представляет параметры защиты листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e32e41eb46cc5af98f6d9aeffcf470e22fbad349
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523723"
---
# <a name="worksheetprotectionoptions-resource-type"></a>Тип ресурса WorksheetProtectionOptions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры защиты листа.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowAutoFilter|логический|Представляет параметр защиты листа, разрешающий использовать функцию автофильтра.|
|allowDeleteColumns|логический|Представляет параметр защиты листа, разрешающий удалять столбцы.|
|allowDeleteRows|логический|Представляет параметр защиты листа, разрешающий удалять строки.|
|allowFormatCells|логический|Представляет параметр защиты листа, разрешающий форматировать ячейки.|
|allowFormatColumns|логический|Представляет параметр защиты листа, разрешающий форматировать столбцы.|
|allowFormatRows|логический|Представляет параметр защиты листа, разрешающий форматировать строки.|
|allowInsertColumns|логический|Представляет параметр защиты листа, разрешающий вставлять столбцы.|
|allowInsertHyperlinks|логический|Представляет параметр защиты листа, разрешающий вставлять гиперссылки.|
|allowInsertRows|логический|Представляет параметр защиты листа, разрешающий вставлять строки.|
|allowPivotTables|логический|Представляет параметр защиты листа, разрешающий использовать функцию сводных таблиц.|
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
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheetprotectionoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
