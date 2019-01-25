---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517633"
---
# <a name="itemactivitystat-resource-type"></a>Тип ресурса itemActivityStat

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **itemActivityStat** содержит сведения о действиях, выполняемых в течение интервала времени.

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

| Свойство         | Тип                    | Описание
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | Указывает, что Статистика ожидания основаны на неполные данные. Только для чтения.
| isTrending       | Логическое                 | Указывает, является ли элемент «прибора.» Только для чтения.
| startDateTime    | DateTimeOffset          | При запуске интервала. Только для чтения.
| endDateTime      | DateTimeOffset          | Окончания интервала. Только для чтения.
| create           | [itemActionStat][]      | Сведения о действия **Создание** ожидания. Только для чтения.
| edit             | [itemActionStat][]      | Сведения о действия **редактирования** в этот интервал. Только для чтения.
| delete           | [itemActionStat][]      | Сведения о действиям **удаления** ожидания. Только для чтения.
| move             | [itemActionStat][]      | Сведения о действия **переместить** в этот интервал. Только для чтения.
| Access           | [itemActionStat][]      | Сведения о действия **клиента** в этот интервал. Только для чтения.

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Связи

| Имя связи | Тип                        | Описание
|:------------------|:----------------------------|:---------------------------
| activities        | Коллекция [itemActivity][] | Предоставляет **itemActivities** , представленного в этом **itemActivityStat** ресурсов.

[itemActivity]: itemactivity.md

## <a name="remarks"></a>Замечания

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitystat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
