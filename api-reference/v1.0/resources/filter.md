---
title: Тип ресурса Filter
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0d3204213fe70fa66cd9fac569a5c4629a414a780b65e8e8d6f238b901a4a2ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205824"
---
# <a name="filter-resource-type"></a>Тип ресурса Filter

Пространство имен: microsoft.graph

Управляет фильтрацией столбца таблицы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Apply](../api/filter-apply.md)|Нет|Применяет заданные условия фильтра для определенного столбца.|
|[Clear](../api/filter-clear.md)|Нет|Сбрасывает фильтр для определенного столбца.|

## <a name="properties"></a>Свойства

| Имя | Тип   |Описание|
|:---------------|:--------|:----------|
|criteria|[WorkbookFilterCriteria](filtercriteria.md)|Текущий фильтр, заданный для определенного столбца. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

