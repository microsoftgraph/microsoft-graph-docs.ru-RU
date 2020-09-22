---
title: Тип ресурса Chart
description: Представляет объект диаграммы в книге.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2aedb1869a0dee1cc9e0d13fa85ca3c06bcc1d1c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032826"
---
# <a name="chart-resource-type"></a>Тип ресурса Chart

Пространство имен: microsoft.graph

Представляет объект диаграммы в книге.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта Chart](../api/chart-get.md) | [WorkbookChart](chart.md) |Чтение свойств и связей объекта диаграммы.|
|[Создание объекта ChartSeries](../api/chart-post-series.md) |[воркбукчартсериес](chartseries.md)| Создание объекта ChartSeries путем добавления в коллекцию рядов.|
|[Список рядов](../api/chart-list-series.md) |Коллекция [воркбукчартсериес](chartseries.md)| Получение коллекции объектов ChartSeries.|
|[Обновление](../api/chart-update.md) | [WorkbookChart](chart.md)   |Обновление объекта Chart. |
|[Image](../api/chart-image.md)|Строка изображения с кодировкой base64|Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.|
|[удаление](../api/chart-delete.md);|Нет|Удаляет объект диаграммы.|
|[Setdata](../api/chart-setdata.md)|Нет|Сбрасывает исходные данные для диаграммы.|
|[Setposition](../api/chart-setposition.md)|Нет|Располагает диаграмму относительно ячеек на листе.|
|[Список](../api/chart-list.md) | Коллекция [WorkbookChart](chart.md) |Получение коллекции объектов диаграмм. |
|[Itemat](../api/chartcollection-itemat.md)|[WorkbookChart](chart.md)|Возвращает диаграмму с учетом ее положения в коллекции.|
|[Add](../api/chartcollection-add.md)|[WorkbookChart](chart.md)|Создает диаграмму.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|height|double|Обозначает высоту объекта диаграммы (в пунктах).|
|id|string|Возвращает диаграмму с учетом ее положения в коллекции. Только для чтения.|
|left|double|Расстояние в пунктах от левого края диаграммы до начала листа.|
|name|string|Обозначает имя объекта диаграммы.|
|top|double|Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).|
|width|double|Представляет ширину объекта диаграммы (в пунктах).|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|axes|[воркбукчартаксес](chartaxes.md)|Представляет оси диаграммы. Только для чтения.|
|dataLabels|[воркбукчартдаталабелс](chartdatalabels.md)|Представляет метки данных на диаграмме. Только для чтения.|
|format|[воркбукчартареаформат](chartareaformat.md)|Инкапсулирует свойства формата для области диаграммы. Только для чтения.|
|legend|[воркбукчартлеженд](chartlegend.md)|Представляет условные обозначения для диаграммы. Только для чтения.|
|series|Коллекция [воркбукчартсериес](chartseries.md)|Представляет один ряд данных или коллекцию рядов данных в диаграмме. Только для чтения.|
|title|[воркбукчарттитле](charttitle.md)|Представляет заголовок указанной диаграммы, включая его текст, видимость, положение и форматирование. Только для чтения.|
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

