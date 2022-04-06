---
author: daspek
description: Ресурс itemActivityStat предоставляет сведения о действиях, которые произошли в интервале времени.
ms.date: 09/14/2017
title: ItemActivityStat
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 27089dcb5e9223710edb60bbdafe88fa0b3f8099
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723907"
---
# <a name="itemactivitystat-resource-type"></a>тип ресурса itemActivityStat

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **itemActivityStat** предоставляет сведения о действиях, которые произошли в интервале времени.

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

## <a name="properties"></a>Свойства

| Свойство       | Тип               | Описание                                                                             |
| :------------- | :----------------- | :-------------------------------------------------------------------------------------- |
| incompleteData | [incompleteData][] | Указывает, что статистика в этом интервале основана на неполных данных. Только для чтения. |
| isTrending     | Boolean            | Указывает, является ли элемент "трендом". Только для чтения.                                    |
| startDateTime  | DateTimeOffset     | Когда начинается интервал. Только для чтения.                                                    |
| endDateTime    | DateTimeOffset     | Когда интервал заканчивается. Только для чтения.                                                      |
| create         | [itemActionStat][] | Статистика создания **действий** в этом интервале. Только для чтения.                    |
| edit           | [itemActionStat][] | Статистика действий **редактирования** в этом интервале. Только для чтения.                      |
| delete         | [itemActionStat][] | Статистика действий **удаления в** этом интервале. Только для чтения.                    |
| move           | [itemActionStat][] | Статистика действий **перемещения** в этом интервале. Только для чтения.                      |
| доступ         | [itemActionStat][] | Статистика действий **доступа** в этом интервале. Только для чтения.                    |

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Связи

| Связь | Тип                        | Описание                                                                       |
| :----------- | :-------------------------- | :-------------------------------------------------------------------------------- |
| activities   | Коллекция [itemActivity][] | Предоставляет **itemActivities** , представленные в этом **ресурсе itemActivityStat** . |

[itemActivity]: itemactivity.md

## <a name="remarks"></a>Замечания

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": []
}
-->
