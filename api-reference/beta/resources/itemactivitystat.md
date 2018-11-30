---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
ms.openlocfilehash: 067cf88773b5f5d69b2b3538a2ddeab6741631a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075135"
---
# <a name="itemactivitystat-resource-type"></a>Тип ресурса itemActivityStat

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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

| Свойство         | Тип                    | Description
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | Указывает, что Статистика ожидания основаны на неполные данные. Только для чтения.
| isTrending       | Логический                 | Указывает, является ли элемент «прибора.» Только для чтения.
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

## <a name="remarks"></a>Примечания

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
