---
author: daspek
title: тип ресурса itemActionStat
description: Объект itemActionStat предоставляет сводные сведения о действии в течение определенного периода времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 595a479f98e6327f3e43c2278c646d6e570e5a290cdcae8b7151ac4162d15578
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246677"
---
# <a name="itemactionstat-resource-type"></a>тип ресурса itemActionStat

Пространство имен: microsoft.graph

Ресурс **itemActionStat** предоставляет сводные сведения о действии в течение определенного периода времени.

## <a name="properties"></a>Свойства

| Свойство    | Тип  | Описание
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | Количество действий. Только для чтения.
| actorCount  | Int32 | Количество различных субъектов, которые выполняли действие. Только для чтения.

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

