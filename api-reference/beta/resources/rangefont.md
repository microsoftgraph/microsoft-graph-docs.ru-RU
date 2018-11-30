---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
ms.openlocfilehash: fc1f3e35bb2ea612dd462d97075ad9757e27bf22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075456"
---
# <a name="rangefont-resource-type"></a>Тип ресурса RangeFont

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeFont](../api/rangefont-get.md) | [RangeFont](rangefont.md) |Чтение свойств и связей объекта rangeFont.|
|[Update](../api/rangefont-update.md) | [RangeFont](rangefont.md)   |Обновление объекта RangeFont. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bold|boolean|Указывает, является ли шрифт полужирным.|
|color|строка|HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.|
|italic|boolean|Указывает, применяется ли курсив.|
|name|строка|Имя шрифта (например, Calibri)|
|size|double|font-size|
|underline|строка|Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->