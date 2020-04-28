---
title: Тип ресурса Воркбукворкшитпротектион
description: Представляет защиту объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ab5d3101b1b9cabf8843d3726f036de74bf3a258
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519101"
---
# <a name="workbookworksheetprotection-resource-type"></a>Тип ресурса Воркбукворкшитпротектион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет защиту объекта листа.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбукворкшитпротектион](../api/worksheetprotection-get.md) | [воркбукворкшитпротектион](workbookworksheetprotection.md) |Чтение свойств и связей объекта Воркбукворкшитпротектион.|
|[Protect](../api/worksheetprotection-protect.md)|Нет|Защита листа. Выдает исключение, если лист защищен.|
|[Unprotect](../api/worksheetprotection-unprotect.md)|Нет|Снятие защиты с листа|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|options|[воркбукворкшитпротектионоптионс](workbookworksheetprotectionoptions.md)|Параметры защиты листа. Только для чтения.|
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
