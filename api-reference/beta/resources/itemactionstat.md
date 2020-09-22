---
author: daspek
description: Ресурс Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
ms.date: 09/14/2017
title: итемактионстат
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8316239a7e00cdc74921c42b70431eba60cdc2d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075680"
---
# <a name="itemactionstat-resource-type"></a>Тип ресурса Итемактионстат

Пространство имен: microsoft.graph

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
| актионкаунт | Int32 | Количество попыток выполнения действия. Только для чтения.
| акторкаунт  | Int32 | Количество уникальных субъектов, которые выполнили действие. Только для чтения.

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


