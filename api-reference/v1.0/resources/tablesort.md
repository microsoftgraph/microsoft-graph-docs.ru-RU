---
title: Тип ресурса TableSort
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d56d739a51b78ad7fdfd9f5cc8033b544ebb87ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835079"
---
# <a name="tablesort-resource-type"></a>Тип ресурса TableSort

Управляет операциями сортировки для объектов Table.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableSort](../api/tablesort-get.md) | [WorkbookTableSort](tablesort.md) |Чтение свойств и связей объекта tableSort.|
|[Apply](../api/tablesort-apply.md)|Нет|Выполняет сортировку.|
|[Clear](../api/tablesort-clear.md)|Нет|Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.|
|[Reapply](../api/tablesort-reapply.md)|Нет|Повторно применяет текущие параметры сортировки к таблице.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fields|[WorkbookSortField](sortfield.md) коллекции|Указывает текущие условия, которые использовались при последней сортировке таблицы. Только для чтения.|
|matchCase|boolean|Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.|
|method|string|Представляет порядка способ, используемый для сортировки в таблице последнего китайских знаков. Возможные значения: `PinYin`, `StrokeCount`. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
