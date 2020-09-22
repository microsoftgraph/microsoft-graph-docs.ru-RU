---
title: Тип ресурса ChartTitle
description: Представляет объект заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b6325656dcf11a4b448506f829c3aaae88100ce6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059224"
---
# <a name="charttitle-resource-type"></a>Тип ресурса ChartTitle

Пространство имен: microsoft.graph

Представляет объект заголовка диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartTitle](../api/charttitle-get.md) | [воркбукчарттитле](charttitle.md) |Чтение свойств и связей объекта chartTitle.|
|[Обновление](../api/charttitle-update.md) | [воркбукчарттитле](charttitle.md)    |Обновление объекта ChartTitle. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|overlay|boolean|Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.|
|text|string|Представляет текст заголовка диаграммы.|
|visible|boolean|Логическое значение, представляющее видимость объекта заголовка диаграммы.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[воркбукчарттитлеформат](charttitleformat.md)|Представляет форматирование названия диаграммы, включая формат заливки и шрифта. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

