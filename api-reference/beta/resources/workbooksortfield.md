---
title: Тип ресурса Воркбуксортфиелд
description: Представляет условие в операции сортировки.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: adcebc20b39d40ef283d25cfd2a8c247160580eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519143"
---
# <a name="workbooksortfield-resource-type"></a>Тип ресурса Воркбуксортфиелд

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет условие в операции сортировки.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ascending|boolean|Указывает, выполняется ли сортировка по возрастанию.|
|color|строка|Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.|
|dataOption|string|Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal`, `TextAsNumber`.|
|key|int|Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).|
|sortOn|string|Представляет тип сортировки этого условия. Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|icon|[воркбукикон](workbookicon.md)|Представляет значок, определенный условием, при сортировке по значку ячейки.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
