---
title: Тип ресурса Планнерпланконтекст
description: Ресурс **планнерпланконтекст** представляет связь plannerPlan с возможностями взаимодействия с пользователем вне планировщика. Планы планировщика могут быть предоставлены в других интерфейсах, таких как Microsoft Teams, для отслеживания работы в контексте этого интерфейса.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 68d9233d2645c2176ad364fbcbfac869976f0586
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344454"
---
# <a name="plannerplancontext-resource-type"></a>Тип ресурса Планнерпланконтекст

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **планнерпланконтекст** представляет связь [plannerPlan](plannerplan.md) с возможностями взаимодействия с пользователем вне планировщика. Планы планировщика могут быть предоставлены в других интерфейсах, таких как Microsoft Teams, для отслеживания работы в контексте этого интерфейса.
Интерфейс повторной отправки записи **планнерпланконтекст** можно определить на основе свойства **овнераппид** :
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: Контекстная запись относится к Microsoft Teams.
 - является 00000003-0000-0ff1-ce00-000000000000: запись контекста принадлежит SharePoint.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Типе|String|Допускает значение null. Определяемый приложением тип связи между [plannerPlan](plannerplan.md) и приложением. Приложение может использовать эту информацию для отслеживания различных видов отношений с одним и тем же [plannerPlan](plannerplan.md).|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания **планнерпланконтекст** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Дисплайнамесегментс|Коллекция String|Сегменты имени внешнего интерфейса взаимодействия. Сегменты представляют иерархическую структуру, которая позволяет другим приложениям отображать связь.|
|Овнераппид|String|Только для чтения. Идентификатор приложения, создавшего **планнерпланконтекст**.|

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
  "suppressions": []
}
-->
