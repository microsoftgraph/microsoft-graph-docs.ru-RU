---
author: daspek
title: тип ресурса itemActivityStat
description: Объект ItemActivityStat предоставляет сведения о действиях, которые произошли на элементе.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 97702f31f8b6125b06d3c34eba9eda596604422c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113667"
---
# <a name="itemactivitystat-resource-type"></a>тип ресурса itemActivityStat

Пространство имен: microsoft.graph

Ресурс **itemActivityStat** предоставляет сведения о действиях, которые произошли в интервале времени.

## <a name="properties"></a>Свойства

| Свойство         | Тип                    | Описание
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | Указывает, что статистика в этом интервале основана на неполных данных. Только для чтения.
| isTrending       | Логический                 | Указывает, является ли элемент "трендом". Только для чтения.
| startDateTime    | DateTimeOffset          | Когда начинается интервал. Только для чтения.
| endDateTime      | DateTimeOffset          | Когда интервал заканчивается. Только для чтения.
| create           | [itemActionStat][]      | Статистика создания **действий** в этом интервале. Только для чтения.
| edit             | [itemActionStat][]      | Статистика действий **редактирования** в этом интервале. Только для чтения.
| delete           | [itemActionStat][]      | Статистика действий **удаления в** этом интервале. Только для чтения.
| move             | [itemActionStat][]      | Статистика действий **перемещения** в этом интервале. Только для чтения.
| доступ           | [itemActionStat][]      | Статистика действий **доступа** в этом интервале. Только для чтения.

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Связи

| Имя связи | Тип                        | Описание
|:------------------|:----------------------------|:---------------------------
| activities        | Коллекция [itemActivity][] | Предоставляет **itemActivities,** представленные в этом **ресурсе itemActivityStat.**

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

