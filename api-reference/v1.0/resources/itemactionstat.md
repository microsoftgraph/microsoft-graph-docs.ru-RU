---
author: daspek
title: тип ресурса itemActionStat
description: Объект itemActionStat предоставляет сводные сведения о действии в течение определенного периода времени.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 047ffe54a613cafbe953a4ff72794382ab440b7e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104126"
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

