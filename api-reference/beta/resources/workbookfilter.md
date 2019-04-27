---
title: Тип ресурса Воркбукфилтер
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
ms.openlocfilehash: 79ded0bfca0ace3b2d7c1bcdb4cd8dd2696802a4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33349002"
---
# <a name="workbookfilter-resource-type"></a>Тип ресурса Воркбукфилтер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управляет фильтрацией столбца таблицы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Apply](../api/filter-apply.md)|Нет|Применяет заданные условия фильтра для определенного столбца.|
|[Clear](../api/filter-clear.md)|Нет|Сбрасывает фильтр для определенного столбца.|

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|criteria|[Воркбукфилтеркритериа](workbookfiltercriteria.md)|Текущий фильтр, заданный для определенного столбца. Только для чтения.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
    "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
