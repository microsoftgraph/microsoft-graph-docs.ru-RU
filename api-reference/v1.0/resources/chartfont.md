---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3862a6273e9dfca4df6bb412afcc061b057e617c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069199"
---
# <a name="chartfont-resource-type"></a>Тип ресурса ChartFont

Пространство имен: microsoft.graph

Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartFont](../api/chartfont-get.md) | [воркбукчартфонт](chartfont.md) |Чтение свойств и связей объекта chartFont.|
|[Обновление](../api/chartfont-update.md) | [воркбукчартфонт](chartfont.md)   |Обновление объекта ChartFont. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bold|boolean|Указывает, является ли шрифт полужирным.|
|color|string|HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.|
|italic|boolean|Указывает, применяется ли курсив.|
|name|string|Имя шрифта (например, Calibri)|
|size|Double|Размер шрифта (например, 11)|
|underline|string|Тип подчеркивания, применяемый для шрифта. Возможные значения: `None` , `Single` .|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

