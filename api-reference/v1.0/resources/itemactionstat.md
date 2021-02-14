---
author: daspek
title: Тип ресурса itemActionStat
description: Объект itemActionStat предоставляет сводные сведения о действии за период времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 13bc306a1b14d7d59ec8eddda5b02a5cba84e649
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238528"
---
# <a name="itemactionstat-resource-type"></a>Тип ресурса itemActionStat

Пространство имен: microsoft.graph

Ресурс **itemActionStat** предоставляет сводную информацию о действии за период времени.

## <a name="properties"></a>Свойства

| Свойство    | Тип  | Описание
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | Количество действий. Только для чтения.
| actorCount  | Int32 | Количество отдельных субъектов, которые выполнили действие. Только для чтения.

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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/itemActionStat",
  "suppressions": []
}
-->

