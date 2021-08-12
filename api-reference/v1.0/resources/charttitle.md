---
title: Тип ресурса ChartTitle
description: Представляет объект заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3fc42cb04a12dbe1c8a792c4d9c6af4ad8e5ff0f68b8dd8fe2402990909db26b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178544"
---
# <a name="charttitle-resource-type"></a>Тип ресурса ChartTitle

Пространство имен: microsoft.graph

Представляет объект заголовка диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartTitle](../api/charttitle-get.md) | [КнигаChartTitle](charttitle.md) |Чтение свойств и связей объекта chartTitle.|
|[Обновление](../api/charttitle-update.md) | [КнигаChartTitle](charttitle.md)    |Обновление объекта ChartTitle. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|overlay|boolean|Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.|
|text|string|Представляет текст заголовка диаграммы.|
|visible|boolean|Логическое значение, представляющее видимость объекта заголовка диаграммы.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[WorkbookChartTitleFormat](charttitleformat.md)|Представляет форматирование названия диаграммы, включая формат заливки и шрифта. Только для чтения.|

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

