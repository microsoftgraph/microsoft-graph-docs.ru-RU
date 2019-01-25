---
title: Тип ресурса plannerRecentPlanReferenceCollection
description: Ресурс **plannerRecentPlanReferenceCollection** представляет коллекцию ссылок на планы, которые были недавно просмотре пользователем. Этот ресурс является открытым и является частью объекта plannerUser. Имя свойства — это идентификатор соответствующего плана. Значение в паре значение свойства — это объект plannerRecentPlanReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e27375e3f2395b3528873d8b83f0b5aa6f48d52e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514994"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>Тип ресурса plannerRecentPlanReferenceCollection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerRecentPlanReferenceCollection** представляет коллекцию ссылок на планы, которые были недавно просмотре пользователем. Этот ресурс является открытым и является частью объекта [plannerUser](planneruser.md) . Имя свойства — это идентификатор соответствующего плана. Значение в паре значение свойства — это объект [plannerRecentPlanReference](plannerrecentplanreference.md) .
Добавление новой ссылки для данного семейства сайтов автоматическое удаление старых записей, при превышении предопределенное значение максимального размера семейства.


## <a name="properties"></a>Свойства
Можно определить свойства этого типа open. Имена свойств являются `id` значений [plannerPlan](plannerplan.md) ресурсов и их значения должны быть [plannerRecentPlanReference](plannerrecentplanreference.md) объектов. Чтобы удалить элемент в списке "Избранное", задайте значение свойства, которое должно `null`.


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
}-->

```json
{
  "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-02T22:49:46.155Z",
    "planTitle": "Purchase Workflow"
  },
  "iKNMHkk3vEWpSF7F7iZWIGQAAMMw": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-03T21:59:28.975Z",
    "planTitle": "New Year's Office Party"
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
