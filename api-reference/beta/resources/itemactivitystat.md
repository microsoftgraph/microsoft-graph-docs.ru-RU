---
author: daspek
description: Ресурс itemActivityStat предоставляет сведения о действиях, выполненных в течение интервала времени.
ms.date: 09/14/2017
title: ItemActivityStat
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: c5dbf0235abda09ec56abb8ac450d15b8836f4ba
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176857"
---
# <a name="itemactivitystat-resource-type"></a>Тип ресурса itemActivityStat

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **itemActivityStat** предоставляет сведения о действиях, выполненных в течение интервала времени.

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
| isTrending     | Логическое            | Указывает, является ли элемент "трендом". Только для чтения.                                    |
| startDateTime  | DateTimeOffset     | При запуске интервала. Только для чтения.                                                    |
| endDateTime    | DateTimeOffset     | Когда интервал заканчивается. Только для чтения.                                                      |
| create         | [itemActionStat][] | Статистика действий **создания в** этом интервале. Только для чтения.                    |
| edit           | [itemActionStat][] | Статистика действий **редактирования** в этом интервале. Только для чтения.                      |
| delete         | [itemActionStat][] | Статистика действий **удаления в** этом интервале. Только для чтения.                    |
| move           | [itemActionStat][] | Статистика действий **перемещения в** этом интервале. Только для чтения.                      |
| Доступа         | [itemActionStat][] | Статистика действий **доступа в** этом интервале. Только для чтения.                    |

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Связи

| Связь | Тип                        | Описание                                                                       |
| :----------- | :-------------------------- | :-------------------------------------------------------------------------------- |
| activities   | Коллекция [itemActivity][] | Предоставляет объект **itemActivities** , представленный в этом **ресурсе itemActivityStat** . |

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
