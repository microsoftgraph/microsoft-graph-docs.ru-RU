---
title: Тип ресурса plannerRecentPlanReference
description: 'Ресурс **plannerRecentPlanReference** введите repesents ссылку на plannerPlan, недавно просмотренный пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bafaf6d20dc8f64ffe49eb4e2f998607708a2773
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943532"
---
# <a name="plannerrecentplanreference-resource-type"></a>Тип ресурса plannerRecentPlanReference

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerRecentPlanReference** введите repesents ссылку на [plannerPlan](plannerplan.md) , недавно просмотренный пользователя. **PlannerRecentPlanReferences** для пользователя, явно задаваемые с помощью приложения. Все приложения, которое реализует функцию последние планы следует записать при соответствующим образом пользователь последнего просмотра записи **plannerRecentPlanReference** обновления и плана.
Приложения следует иметь в виду, что записи **plannerRecentPlanReference** можно ссылаться на **plannerPlans** , будут удалены, пользователь больше не может получить доступ и добавлены иное название.
Рекомендуется уведомлять пользователей есть несоответствия приложений и обновлять записи.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|Дата и время, планирование последнего просмотра пользователем. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|planTitle|Строка|Название плана во время пользователь просматривать его.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
