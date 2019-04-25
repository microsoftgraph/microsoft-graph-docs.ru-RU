---
title: Тип ресурса ChartAxisTitleFormat
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26d305d8bd4a0059123f77bd86cbbf5fd01dcea7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569083"
---
# <a name="chartaxistitleformat-resource-type"></a>Тип ресурса ChartAxisTitleFormat

Представляет форматирование для названий осей диаграммы.


## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|font|[Воркбукчартфонт](chartfont.md)|Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д. объект заголовка оси диаграммы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
