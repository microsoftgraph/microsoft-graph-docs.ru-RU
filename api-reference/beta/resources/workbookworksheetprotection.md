---
title: Тип ресурса Воркбукворкшитпротектион
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e4a2f3130c71df35b1106d1a342004cfc6fdf25
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348958"
---
# <a name="workbookworksheetprotection-resource-type"></a>Тип ресурса Воркбукворкшитпротектион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет защиту объекта листа.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбукворкшитпротектион](../api/worksheetprotection-get.md) | [Воркбукворкшитпротектион](workbookworksheetprotection.md) |Чтение свойств и связей объекта Воркбукворкшитпротектион.|
|[Protect](../api/worksheetprotection-protect.md)|Отсутствует|Защита листа. Выдает исключение, если лист защищен.|
|[Unprotect](../api/worksheetprotection-unprotect.md)|Нет|Снятие защиты с листа|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|options|[Воркбукворкшитпротектионоптионс](workbookworksheetprotectionoptions.md)|Параметры защиты листа. Только для чтения.|
|protected|boolean|Указывает, защищен ли лист.  Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "options"
  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": "boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
