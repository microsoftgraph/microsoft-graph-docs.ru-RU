---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Итемактионстат
localization_priority: Normal
ms.openlocfilehash: a0e3bc3f217308d96eaadf6ab367431c7f1b8c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345454"
---
# <a name="itemactionstat-resource-type"></a>Тип ресурса Итемактионстат

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.

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
| Актионкаунт | Int32 | Количество попыток выполнения действия. Только для чтения.
| Акторкаунт  | Int32 | Количество уникальных субъектов, которые выполнили действие. Только для чтения.

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
