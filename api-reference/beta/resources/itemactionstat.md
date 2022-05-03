---
author: daspek
description: Ресурс itemActionStat предоставляет агрегатные сведения о действии за период времени.
ms.date: 09/14/2017
title: ItemActionStat
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: b1fb726904c3b97ead34162410025a82f410231d
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176300"
---
# <a name="itemactionstat-resource-type"></a>Тип ресурса itemActionStat

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **itemActionStat** предоставляет агрегатные сведения о действии за период времени.

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

## <a name="properties"></a>Свойства

| Свойство    | Тип  | Описание
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | Количество выполненных действий. Только для чтения.
| actorCount  | Int32 | Количество различных субъектов, которые выполнили действие. Только для чтения.

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": []
}
-->


