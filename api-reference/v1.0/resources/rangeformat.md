---
title: Тип ресурса RangeFormat
description: Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.
localization_priority: Normal
ms.openlocfilehash: 86ec37ffa85d7d9785b6a2f632ff3f337ce0e734
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823809"
---
# <a name="rangeformat-resource-type"></a>Тип ресурса RangeFormat

Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeFormat](../api/rangeformat-get.md) | [WorkbookRangeFormat](rangeformat.md) |Чтение свойств и связей объекта rangeFormat.|
|[Создание объекта RangeBorder](../api/rangeformat-post-borders.md) |[WorkbookRangeBorder](rangeborder.md)| Создание объекта RangeBorder путем добавления в коллекцию границ.|
|[Список границ](../api/rangeformat-list-borders.md) |[WorkbookRangeBorder](rangeborder.md) коллекции| Получение коллекции объектов RangeBorder.|
|[обновление](../api/rangeformat-update.md). | [WorkbookRangeFormat](rangeformat.md) |Обновление объекта RangeFormat. |
|[Autofitcolumns](../api/rangeformat-autofitcolumns.md)|Нет|Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.|
|[Autofitrows](../api/rangeformat-autofitrows.md)|Нет|Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|columnWidth|double|Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.|
|horizontalAlignment|string|Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.|
|rowHeight|double|Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.|
|verticalAlignment|string|Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.|
|wrapText|boolean|Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|borders|[WorkbookRangeBorder](rangeborder.md) коллекции|Коллекция объектов границ, которые применяются к общему выделенному диапазону. Только для чтения.|
|fill|[WorkbookRangeFill](rangefill.md)|Возвращает объект заливки, определенный для всего диапазона. Только для чтения.|
|font|[WorkbookRangeFont](rangefont.md)|Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.|
|protection|[WorkbookFormatProtection](formatprotection.md)|Возвращает объект защиты формата для диапазона. Только для чтения.|

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
