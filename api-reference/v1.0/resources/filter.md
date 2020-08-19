---
title: Тип ресурса Filter
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ecaa61bde452d13e7e8e7fe0c79e3b75eeaa591a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807810"
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
|criteria|[воркбукфилтеркритериа](filtercriteria.md)|Текущий фильтр, заданный для определенного столбца. Только для чтения.|

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
