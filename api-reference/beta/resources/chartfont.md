---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4187d2837835520864ec3a1ef5c47b578b3d3da4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920949"
---
# <a name="chartfont-resource-type"></a>Тип ресурса ChartFont

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartFont](../api/chartfont-get.md) | [ChartFont](chartfont.md) |Чтение свойств и связей объекта chartFont.|
|[обновление](../api/chartfont-update.md). | [ChartFont](chartfont.md)   |Обновление объекта ChartFont. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bold|boolean|Указывает, является ли шрифт полужирным.|
|color|строка|HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.|
|italic|boolean|Указывает, применяется ли курсив.|
|name|строка|Имя шрифта (например, Calibri)|
|size|Double|Размер шрифта (например, 11)|
|underline|строка|Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
