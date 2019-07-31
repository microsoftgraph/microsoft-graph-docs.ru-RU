---
title: Тип ресурса Воркбукранжефонт
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b3982a8026cd720fe614b11405a37bed8626042d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964053"
---
# <a name="workbookrangefont-resource-type"></a>Тип ресурса Воркбукранжефонт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбукранжефонт](../api/rangefont-get.md) | [Воркбукранжефонт](workbookrangefont.md) |Чтение свойств и связей объекта rangeFont.|
|[Обновление](../api/rangefont-update.md) | [Воркбукранжефонт](workbookrangefont.md)   |Обновление объекта RangeFont. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bold|boolean|Указывает, является ли шрифт полужирным.|
|color|строка|HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.|
|italic|boolean|Указывает, применяется ли курсив.|
|name|string|Имя шрифта (например, Calibri)|
|size|double|размер шрифта|
|underline| String |Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
