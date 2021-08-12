---
title: Тип ресурса WorksheetProtection
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f69409c3bcab7eaa91e08341f5b81074589ca64e7fb83c56b48f30e451fc736f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163616"
---
# <a name="worksheetprotection-resource-type"></a>Тип ресурса WorksheetProtection

Пространство имен: microsoft.graph

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
|options|[workbookWorksheetProtectionOptions](worksheetprotectionoptions.md)|Параметры защиты листа. Только для чтения.|
|protected|boolean|Указывает, защищен ли лист.  Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

