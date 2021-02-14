---
author: daspek
title: Тип ресурса itemActivityStat
description: Объект ItemActivityStat предоставляет сведения о действиях, которые произошли с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a33453fc884fc6dba7bd5b8fbcf4edc0261c11cb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238682"
---
# <a name="itemactivitystat-resource-type"></a>Тип ресурса itemActivityStat

Пространство имен: microsoft.graph

Ресурс **itemActivityStat** предоставляет сведения о действиях, которые произошли в течение интервала времени.

## <a name="properties"></a>Свойства

| Свойство         | Тип                    | Описание
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | Указывает, что статистика за этот интервал основана на неполных данных. Только для чтения.
| isTrending       | Логическое                 | Указывает, является ли элемент "трендом". Только для чтения.
| startDateTime    | DateTimeOffset          | Когда начинается интервал. Только для чтения.
| endDateTime      | DateTimeOffset          | Когда интервал заканчивается. Только для чтения.
| create           | [itemActionStat][]      | Статистика о действиях **создания** за этот интервал. Только для чтения.
| edit             | [itemActionStat][]      | Статистика о действиях **редактирования** за этот интервал. Только для чтения.
| delete           | [itemActionStat][]      | Статистика о действиях **удаления** за этот интервал. Только для чтения.
| move             | [itemActionStat][]      | Статистика о действиях **перемещения** за этот интервал. Только для чтения.
| access           | [itemActionStat][]      | Статистика о действиях **доступа** за этот интервал. Только для чтения.

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Связи

| Имя связи | Тип                        | Описание
|:------------------|:----------------------------|:---------------------------
| activities        | Коллекция [itemActivity][] | Предоставляет объект **itemActivities,** представленный в **ресурсе itemActivityStat.**

[itemActivity]: itemactivity.md

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

