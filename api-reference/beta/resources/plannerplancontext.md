---
title: тип ресурса plannerPlanContext
description: Ресурс **plannerPlanContext** представляет связь планировщикаPlan с пользовательским взаимодействием за пределами Planner. Планы в Planner можно всплыть в других опытах, таких как Microsoft Teams, чтобы отслеживать работу в контексте этого опыта.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8a3b82c35339bb8bc6b3d3d7923b41ed97ecc02
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720986"
---
# <a name="plannerplancontext-resource-type"></a>тип ресурса plannerPlanContext

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerPlanContext** представляет связь планировщикаPlan с пользовательским взаимодействием за пределами Planner. [](plannerplan.md) Планы в Planner можно всплыть в других опытах, таких как Microsoft Teams, чтобы отслеживать работу в контексте этого опыта. В пользовательском интерфейсе можно отображать внешние ссылки в [планировщикеPlanContextDetails,](plannerplancontextdetails.md) что позволяет пользователям посещать эти впечатления.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|associationType|String|Допускается значение null. Определенный приложением тип связи между [планировщикомPlan](plannerplan.md) и приложением. Приложение может использовать эту информацию для отслеживания различных типов отношений с одним и тем же [планировщикомPlan.](plannerplan.md)|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания **планировщикаPlanContext.** Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|displayNameSegments|Коллекция объектов string|Сегменты имени внешнего опыта. Сегменты представляют иерархическую структуру, которая позволяет другим приложениям отображать связь.|
|isCreationContext|Boolean|Только для чтения. Указывает, создается ли план из указанного контекста. Автогенерированная в зависимости от того, задан ли контекст в рамках создания плана.|
|ownerAppId|String|Только для чтения. ID приложения, создав **планировщикPlanContext**.|

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
  "isCreationContext": false,
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
  "suppressions": []
}
-->


