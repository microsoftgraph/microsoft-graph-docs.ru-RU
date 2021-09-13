---
title: Тип ресурса SortField
description: Представляет условие в операции сортировки.
ms.localizationpriority: medium
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ca8acdf09960988cb8da55e45daaf2504ef4e664
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136355"
---
# <a name="sortfield-resource-type"></a>Тип ресурса SortField

Пространство имен: microsoft.graph

Представляет условие в операции сортировки.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ascending|boolean|Указывает, выполняется ли сортировка по возрастанию.|
|color|string|Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.|
|dataOption|string|Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal` , `TextAsNumber` .|
|key|int|Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).|
|sortOn|string|Представляет тип сортировки этого условия. Допустимые значения: `Value`, `CellColor`, `FontColor`, `Icon`.|
|значок|[WorkbookIcon](icon.md)|Представляет значок, определенный условием, при сортировке по значку ячейки.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

