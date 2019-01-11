---
title: Тип ресурсов rangeView
description: Объект rangeView представляет набор видимых ячеек в родительском диапазоне.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c356c737946dc70c6718b71c1c9aa7081069fd96
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859005"
---
# <a name="rangeview-resource-type"></a>Тип ресурсов rangeView

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Объект rangeView представляет набор видимых ячеек в родительском диапазоне.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение списка строк](../api/workbookrangeview-list-rows.md)  |Коллекция [workbookRangeView](workbookrangeview.md)| Получение коллекции объектов workbookRangeView.|
|[Itemat](../api/workbookrangeview-itemat.md)|[workbookRangeView](workbookrangeview.md)|Получение видимой ячейки из диапазона с учетом индекса.|
|[Диапазон](../api/workbookrangeview-range.md)|[workbookRange](range.md)|Возвращение экземпляра range, связанного с ресурсом rangeView.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|columnCount|Int32|Возвращает количество видимых столбцов. Только для чтения.|
|formulas|Json|Представляет формулу в формате A1. |
|formulasLocal|Json|Представляет формулу в формате A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула "=SUM(A1, 1.5)" превратится в "=СУММ(A1;1,5)" на русском языке.    |
|formulasR1C1|Json|Представляет формулу в формате R1C1.   |
|index|Int32|Индекс диапазона.|
|numberFormat|Json|Представляет код в числовом формате Excel для заданной ячейки. Только для чтения. |
|rowCount|Int32|Возвращает количество видимых строк. Только для чтения.  |
|text|Json|Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.    |
|valueTypes|Json|Представляет тип данных каждой ячейки. Только для чтения. Возможные значения: Unknown, Empty, String, Integer, Double, Boolean, Error. |
|values|Json|Представляет необработанные значения указанного объекта rangeView. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.   |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|rows|Коллекция [workbookRangeView](workbookrangeview.md)| Представляет коллекцию видимых ячеек в диапазоне, сопоставленных с указанным диапазоном. Только для чтения.    Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
