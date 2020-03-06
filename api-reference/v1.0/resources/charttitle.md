---
title: Тип ресурса ChartTitle
description: Представляет объект заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2e3d30d1796945c7d0217a83db966a203678f938
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533094"
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
