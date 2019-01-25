---
title: Тип ресурса plannerGroup
description: Ресурс **plannerGroup** предоставляет доступ к ресурсам Планировщика для группы. Он не содержит свойства, которые можно использовать.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84bb20d0b13f9a99db2f8c59b20e0c9c7c87f93f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513783"
---
# <a name="plannergroup-resource-type"></a>Тип ресурса plannerGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerGroup** предоставляет доступ к ресурсам Планировщика для [группы](group.md). Он не содержит свойства, которые можно использовать.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление планов](../api/plannergroup-list-plans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получение коллекции объектов **plannerPlan**.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор объекта **plannerGroup**.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|plans|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускает значение null. Возвращает экземпляры [plannerPlan](plannerplan.md), принадлежащие группе.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
