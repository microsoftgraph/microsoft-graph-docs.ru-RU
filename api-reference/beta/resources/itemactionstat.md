---
author: daspek
description: Ресурс Итемактионстат предоставляет статистические сведения о действии в течение определенного периода времени.
ms.date: 09/14/2017
title: Итемактионстат
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 719a443af65fd9642feee3bc8ddbc832eb3964c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010114"
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
