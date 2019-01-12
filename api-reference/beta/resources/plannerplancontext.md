---
title: Тип ресурса plannerPlanContext
description: Ресурс **plannerPlanContext** представляет отношение plannerPlan взаимодействия с пользователем вне планировщик работы. Планы в планировщике можно отображаются в других каждый раз, такие как группами Майкрософт, для отслеживания работ в контексте этот опыт.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e118e32ea74332f0d8d0f958f7c55cd9980acb8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962893"
---
# <a name="plannerplancontext-resource-type"></a>Тип ресурса plannerPlanContext

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerPlanContext** представляет отношение [plannerPlan](plannerplan.md) взаимодействия с пользователем вне планировщик работы. Планы в планировщике можно отображаются в других каждый раз, такие как группами Майкрософт, для отслеживания работ в контексте этот опыт.
Представляет запись **plannerPlanContext** опытом, можно определить на основе свойства **ownerAppId** .
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: запись контекста относится к группам Майкрософт.
 - 00000003-0000-0ff1-ce00-000000000000: запись контекста относится к SharePoint.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|associationType|Строка|Допускается значение null. Тип связи между [plannerPlan](plannerplan.md) и приложения в определенных приложений. Приложения могут использовать эти сведения для отслеживания различных типов отношений же [plannerPlan](plannerplan.md).|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания **plannerPlanContext** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|displayNameSegments|Коллекция String|Сегменты имя внешнего интерфейса. Сегменты представления иерархической структуры, обеспечивающий другие приложения отобразить отношение.|
|ownerAppId|Строка|Только для чтения. Идентификатор приложения, которые созданы **plannerPlanContext**.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
