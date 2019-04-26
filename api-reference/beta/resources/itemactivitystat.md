---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Итемактивитистат
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561910"
---
# <a name="itemactivitystat-resource-type"></a>Тип ресурса Итемактивитистат

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **итемактивитистат** предоставляет сведения о действиях, которые выполнялись в течение интервала времени.

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
