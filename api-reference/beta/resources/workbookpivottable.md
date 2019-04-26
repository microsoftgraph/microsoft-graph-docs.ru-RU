---
title: Тип ресурса workbookPivotTable
description: Представляет сводную таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 99ad62474ef0c8e56ec5a699edac742ee28ae446
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345791"
---
# <a name="workbookpivottable-resource-type"></a>Тип ресурса workbookPivotTable

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|id|Строка| Идентификатор сводной таблицы.   Только для чтения.|
|name|String|Имя сводной таблицы.    |

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|worksheet|[Воркбукворкшит](workbookworksheet.md)| Лист, содержащий текущую сводную таблицу. Только для чтения.   |

## <a name="json-representation"></a>Представление в формате JSON
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
