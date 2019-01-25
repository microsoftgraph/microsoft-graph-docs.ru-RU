---
title: Тип ресурса plannerPlanContext
description: Ресурс **plannerPlanContext** представляет отношение plannerPlan взаимодействия с пользователем вне планировщик работы. Планы в планировщике можно отображаются в других каждый раз, такие как группами Майкрософт, для отслеживания работ в контексте этот опыт.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 76260b51bc6f77acf6fac22e80bd676edd8b8e11
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509240"
---
# <a name="plannerplancontext-resource-type"></a>Тип ресурса plannerPlanContext

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerPlanContext** представляет отношение [plannerPlan](plannerplan.md) взаимодействия с пользователем вне планировщик работы. Планы в планировщике можно отображаются в других каждый раз, такие как группами Майкрософт, для отслеживания работ в контексте этот опыт.
Представляет запись **plannerPlanContext** опытом, можно определить на основе свойства **ownerAppId** .
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: запись контекста относится к группам Майкрософт.
 - 00000003-0000-0ff1-ce00-000000000000: запись контекста относится к SharePoint.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|associationType|String|Допускается значение null. Тип связи между [plannerPlan](plannerplan.md) и приложения в определенных приложений. Приложения могут использовать эти сведения для отслеживания различных типов отношений же [plannerPlan](plannerplan.md).|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания **plannerPlanContext** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|displayNameSegments|Коллекция String|Сегменты имя внешнего интерфейса. Сегменты представления иерархической структуры, обеспечивающий другие приложения отобразить отношение.|
|ownerAppId|String|Только для чтения. Идентификатор приложения, которые созданы **plannerPlanContext**.|

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontext.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
