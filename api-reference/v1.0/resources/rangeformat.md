---
title: Тип ресурса RangeFormat
description: Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3e1b79c80c20197cc14a5097efdf9eb0513b43e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034890"
---
# <a name="rangeformat-resource-type"></a>Тип ресурса RangeFormat

Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeFormat](../api/rangeformat-get.md) | [WorkbookRangeFormat](rangeformat.md) |Чтение свойств и связей объекта rangeFormat.|
|[Создание объекта RangeBorder](../api/rangeformat-post-borders.md) |[Воркбукранжебордер](rangeborder.md)| Создание объекта RangeBorder путем добавления в коллекцию границ.|
|[Список границ](../api/rangeformat-list-borders.md) |Коллекция [воркбукранжебордер](rangeborder.md)| Получение коллекции объектов RangeBorder.|
|[Обновление](../api/rangeformat-update.md) | [WorkbookRangeFormat](rangeformat.md) |Обновление объекта RangeFormat. |
|[Autofitcolumns](../api/rangeformat-autofitcolumns.md)|Нет|Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.|
|[Autofitrows](../api/rangeformat-autofitrows.md)|Нет|Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|columnWidth|double|Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.|
|horizontalAlignment|string|Представляет выравнивание по горизонтали для указанного объекта. Возможные `General`значения:, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`,. `Distributed`|
|rowHeight|double|Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.|
|verticalAlignment|string|Представляет выравнивание по вертикали для указанного объекта. Допустимые значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.|
|wrapText|boolean|Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|borders|Коллекция [воркбукранжебордер](rangeborder.md)|Коллекция объектов границы, которые применяются к общему выделенному диапазону. Только для чтения.|
|fill|[Воркбукранжефилл](rangefill.md)|Возвращает объект заливки, определенный для всего диапазона. Только для чтения.|
|font|[Воркбукранжефонт](rangefont.md)|Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.|
|protection|[Воркбукформатпротектион](formatprotection.md)|Возвращает объект защиты формата для диапазона. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
