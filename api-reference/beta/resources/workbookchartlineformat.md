---
title: Тип ресурса Воркбукчартлинеформат
description: Инкапсулирует параметры форматирования для элементов линий.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6900b961608ff29c503dc355dfb8876d3e273feb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519297"
---
# <a name="workbookchartlineformat-resource-type"></a>Тип ресурса Воркбукчартлинеформат

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Инкапсулирует параметры форматирования для элементов линий.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбукчартлинеформат](../api/chartlineformat-get.md) | [воркбукчартлинеформат](workbookchartlineformat.md) |Чтение свойств и связей объекта chartLineFormat.|
|[Обновление](../api/chartlineformat-update.md) | [воркбукчартлинеформат](workbookchartlineformat.md) |Обновление объекта ChartLineFormat. |
|[Clear](../api/chartlineformat-clear.md)|Нет|Очищает формат линий элемента диаграммы.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|color|string|HTML-код цвета, представляющий цвет линий в диаграмме.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
