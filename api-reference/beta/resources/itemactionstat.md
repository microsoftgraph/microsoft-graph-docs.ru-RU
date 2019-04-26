---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Итемактионстат
localization_priority: Normal
ms.openlocfilehash: 39209671b63b991a8fb3ccf1c830c8557fce27c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569986"
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
