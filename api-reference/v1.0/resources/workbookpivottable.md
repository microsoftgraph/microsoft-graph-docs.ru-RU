---
title: Тип ресурсов pivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: cdf558abbc0533f1329aed86d5541adf45235cda
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134159"
---
# <a name="pivottable-resource-type"></a>Тип ресурсов pivotTable

Пространство имен: microsoft.graph

Представляет сводную таблицу Excel.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение workbookPivotTable](../api/workbookpivottable-get.md) | [workbookPivotTable](workbookpivottable.md) |Чтение свойств и связей объекта workbookPivotTable.|
|[Refresh](../api/workbookpivottable-refresh.md)|Нет|Обновляет сводную таблицу. |
|[Refreshall](../api/workbookpivottable-refreshall.md)|Нет|Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Идентификатор сводной таблицы.   Только для чтения.|
|name|String|Имя сводной таблицы.    |

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|worksheet|[WorkbookWorksheet](worksheet.md)| Лист, содержащий текущую сводную таблицу. Только для чтения.   |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```

