---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактионстат
description: Объект Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d5531fc969762219f4e2404787190649ecdaf11
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970796"
---
# <a name="itemactionstat-resource-type"></a>Тип ресурса Итемактионстат

Ресурс **итемактионстат** предоставляет статистические сведения о действии в течение определенного периода времени.

## <a name="properties"></a>Свойства

| Свойство    | Тип  | Описание
|:------------|:------|:-------------------------------------------------------
| Актионкаунт | Int32 | Количество попыток выполнения действия. Только для чтения.
| Акторкаунт  | Int32 | Количество уникальных субъектов, которые выполнили действие. Только для чтения.

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
