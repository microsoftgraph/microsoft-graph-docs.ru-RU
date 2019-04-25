---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c507a966dc6b29e46935c5c77a85b557a84cc69c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543733"
---
# <a name="chartfont-resource-type"></a>Тип ресурса ChartFont

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartFont](../api/chartfont-get.md) | [ChartFont](chartfont.md) |Чтение свойств и связей объекта chartFont.|
|[Обновление](../api/chartfont-update.md) | [ChartFont](chartfont.md)   |Обновление объекта ChartFont. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bold|логический|Указывает, является ли шрифт полужирным.|
|color|строка|HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.|
|italic|boolean|Указывает, применяется ли курсив.|
|name|string|Имя шрифта (например, Calibri)|
|size|Double|Размер шрифта (например, 11)|
|underline|string|Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление в формате JSON

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartfont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
