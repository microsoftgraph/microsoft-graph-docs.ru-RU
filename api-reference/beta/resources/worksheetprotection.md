---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6f32ad7b1cc25d9a937f2de68f1bd930d92ec8f9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572936"
---
# <a name="worksheetprotection-resource-type"></a>Тип ресурса WorksheetProtection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет защиту объекта листа.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта WorksheetProtection](../api/worksheetprotection-get.md) | [WorkbookWorksheetProtection](worksheetprotection.md) |Чтение свойств и связей объекта worksheetProtection.|
|[Protect](../api/worksheetprotection-protect.md)|Нет|Защита листа. Выдает исключение, если лист защищен.|
|[Unprotect](../api/worksheetprotection-unprotect.md)|Нет|Снятие защиты с листа|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|protected|boolean|Указывает, защищен ли лист.  Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|options|[workbookWorksheetProtection](worksheetprotectionoptions.md)|Параметры защиты листа. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "options"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheetprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
