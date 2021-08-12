---
title: Тип ресурсов rangeView
description: Объект rangeView представляет набор видимых ячеек в родительском диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8016bd6600a2c220823a2ea53260d41c381b4b9a4b56378888c2e73e49e7116b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251689"
---
# <a name="rangeview-resource-type"></a>Тип ресурсов rangeView

Пространство имен: microsoft.graph RangeView представляет набор видимых ячеек родительского диапазона.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение списка строк](../api/workbookrangeview-list-rows.md) |Коллекция [workbookRangeView](workbookrangeview.md)| Получение коллекции объектов workbookRangeView.|
|[Itemat](../api/workbookrangeview-itemat.md)|[workbookRangeView](workbookrangeview.md)|Получение видимой ячейки из диапазона с учетом индекса.|
|[Диапазон](../api/workbookrangeview-range.md)|[workbookRange](range.md)|Возвращение экземпляра range, связанного с ресурсом rangeView.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|cellAddresses|Json|Представляет адреса ячейки
|columnCount|Int32|Возвращает количество видимых столбцов. Только для чтения.|
|formulas|Json|Представляет формулу в формате A1. |
|formulasLocal|Json|Представляет формулу в формате A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула "=SUM(A1, 1.5)" превратится в "=СУММ(A1;1,5)" на русском языке.    |
|formulasR1C1|Json|Представляет формулу в формате R1C1.   |
|index|Int32|Индекс диапазона.|
|numberFormat|Json|Представляет код в числовом формате Excel для заданной ячейки. Только для чтения. |
|rowCount|Int32|Возвращает количество видимых строк. Только для чтения.  |
|текст|Json|Текстовые значения указанного диапазона. Текстовое значение не зависит от ширины ячейки. Замена знака #, которая происходит в пользовательском интерфейсе Excel, не повлияет на текстовое значение, возвращаемое API. Только для чтения.    |
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
  "baseType": "microsoft.graph.entity",
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
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```

