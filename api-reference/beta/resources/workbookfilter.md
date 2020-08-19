---
title: Тип ресурса Воркбукфилтер
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: 39ebe2f59e5741e4580ef5300400a0b7e480ffad
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808521"
---
# <a name="workbookfilter-resource-type"></a>Тип ресурса Воркбукфилтер

Пространство имен: microsoft.graph

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
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|criteria|[воркбукфилтеркритериа](workbookfiltercriteria.md)|Текущий фильтр, заданный для определенного столбца. Только для чтения.|


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
