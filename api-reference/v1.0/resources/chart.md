---
title: Тип ресурса Chart
description: Представляет объект диаграммы в книге.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 160fcb95fd8ffe4b4d0c2d4e9233afe3492ef32d27b910ee40bb7519b20e591a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121419"
---
# <a name="chart-resource-type"></a>Тип ресурса Chart

Пространство имен: microsoft.graph

Представляет объект диаграммы в книге.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта Chart](../api/chart-get.md) | [WorkbookChart](chart.md) |Чтение свойств и связей объекта диаграммы.|
|[Создание объекта ChartSeries](../api/chart-post-series.md) |[КнигиChartSeries](chartseries.md)| Создание объекта ChartSeries путем добавления в коллекцию рядов.|
|[Список рядов](../api/chart-list-series.md) |[Коллекция книгChartSeries](chartseries.md)| Получение коллекции объектов ChartSeries.|
|[Обновление](../api/chart-update.md) | [WorkbookChart](chart.md)   |Обновление объекта Chart. |
|[Image](../api/chart-image.md)|Строка изображения с кодировкой base64|Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.|
|[Удаление](../api/chart-delete.md)|Нет|Удаляет объект диаграммы.|
|[Setdata](../api/chart-setdata.md)|Нет|Сбрасывает исходные данные для диаграммы.|
|[Setposition](../api/chart-setposition.md)|Нет|Располагает диаграмму относительно ячеек на листе.|
|[Список](../api/chart-list.md) | Коллекция [WorkbookChart](chart.md) |Получение коллекции объектов диаграмм. |
|[Itemat](../api/chartcollection-itemat.md)|[WorkbookChart](chart.md)|Возвращает диаграмму с учетом ее положения в коллекции.|
|[Add](../api/chartcollection-add.md)|[WorkbookChart](chart.md)|Создает диаграмму.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|height|double|Обозначает высоту объекта диаграммы (в пунктах).|
|id|строка|Возвращает диаграмму с учетом ее положения в коллекции. Только для чтения.|
|left|double|Расстояние в пунктах от левого края диаграммы до начала листа.|
|name|string|Обозначает имя объекта диаграммы.|
|top|double|Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).|
|width|double|Представляет ширину объекта диаграммы (в пунктах).|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|axes|[WorkbookChartAxes](chartaxes.md)|Представляет оси диаграммы. Только для чтения.|
|dataLabels|[КнигаChartDataLabels](chartdatalabels.md)|Представляет метки данных на диаграмме. Только для чтения.|
|format|[КнигаChartAreaFormat](chartareaformat.md)|Инкапсулирует свойства формата для области диаграммы. Только для чтения.|
|legend|[КнигаChartLegend](chartlegend.md)|Представляет условные обозначения для диаграммы. Только для чтения.|
|series|[Коллекция книгChartSeries](chartseries.md)|Представляет один ряд данных или коллекцию рядов данных в диаграмме. Только для чтения.|
|title|[КнигаChartTitle](charttitle.md)|Представляет заголовок указанной диаграммы, включая его текст, видимость, положение и форматирование. Только для чтения.|
|worksheet|[WorkbookWorksheet](worksheet.md)|Лист, содержащий текущую диаграмму. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

