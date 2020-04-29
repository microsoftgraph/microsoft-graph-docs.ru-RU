---
author: daspek
ms.author: dspektor
title: Тип ресурса Итемактивитистат
description: Объект Итемактивитистат предоставляет сведения о действиях, выполненных с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 11b19e4b953d4353382aec15071c6589b5bb23c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447670"
---
# <a name="itemactivitystat-resource-type"></a>Тип ресурса Итемактивитистат

Пространство имен: microsoft.graph

Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.

## <a name="properties"></a>Свойства

| Свойство         | Тип                    | Описание
|:-----------------|:------------------------|:----------------------------------------
| инкомплетедата   | [инкомплетедата][]      | Указывает, что статистика в этом интервале основана на неполных данных. Только для чтения.
| Тенденция       | Boolean                 | Указывает, является ли элемент "тенденция". Только для чтения.
| startDateTime    | DateTimeOffset          | Время начала интервала. Только для чтения.
| endDateTime      | DateTimeOffset          | По окончании интервала. Только для чтения.
| create           | [итемактионстат][]      | Статистика по действиям по **созданию** в этом интервале. Только для чтения.
| edit             | [итемактионстат][]      | Статистика действий **редактирования** в этом интервале. Только для чтения.
| delete           | [итемактионстат][]      | Статистика действий **удаления** в этом интервале. Только для чтения.
| move             | [итемактионстат][]      | Статистика действий **перемещения** в этом интервале. Только для чтения.
| обращения           | [итемактионстат][]      | Статистика действий **доступа** в этом интервале. Только для чтения.

[итемактионстат]: itemactionstat.md
[инкомплетедата]: incompletedata.md

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
