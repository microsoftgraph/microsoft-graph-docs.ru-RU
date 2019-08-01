---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактивитистат
description: Объект Итемактивитистат предоставляет сведения о действиях, выполненных с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bf4396e6da5c56b19d33d7a914d864cb6dd54592
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036675"
---
# <a name="itemactivitystat-resource-type"></a>Тип ресурса Итемактивитистат

Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.

## <a name="properties"></a>Свойства

| Свойство         | Тип                    | Описание
|:-----------------|:------------------------|:----------------------------------------
| Инкомплетедата   | [Инкомплетедата][]      | Указывает, что статистика в этом интервале основана на неполных данных. Только для чтения.
| Тенденция       | Boolean                 | Указывает, является ли элемент "тенденция". Только для чтения.
| startDateTime    | DateTimeOffset          | Время начала интервала. Только для чтения.
| endDateTime      | DateTimeOffset          | По окончании интервала. Только для чтения.
| create           | [Итемактионстат][]      | Статистика по действиям по **созданию** в этом интервале. Только для чтения.
| edit             | [Итемактионстат][]      | Статистика действий **редактирования** в этом интервале. Только для чтения.
| delete           | [Итемактионстат][]      | Статистика действий **удаления** в этом интервале. Только для чтения.
| move             | [Итемактионстат][]      | Статистика действий **перемещения** в этом интервале. Только для чтения.
| обращения           | [Итемактионстат][]      | Статистика действий **доступа** в этом интервале. Только для чтения.

[Итемактионстат]: itemactionstat.md
[Инкомплетедата]: incompletedata.md

## <a name="relationships"></a>Связи

| Имя связи | Тип                        | Описание
|:------------------|:----------------------------|:---------------------------
| activities        | Коллекция [itemActivity][] | Предоставляет **итемактивитиес** , представленные в этом ресурсе **итемактивитистат** .

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
