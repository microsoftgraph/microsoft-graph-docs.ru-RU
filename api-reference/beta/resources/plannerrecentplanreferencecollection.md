---
title: Тип ресурса Планнеррецентпланреференцеколлектион
description: Ресурс **планнеррецентпланреференцеколлектион** представляет коллекцию ссылок на планы, которые были недавно просмотрены пользователем. Этот ресурс является открытым типом и является частью объекта plannerUser. Имя свойства — это идентификатор соответствующего плана. Значение в параметре "свойство-значение" является объектом Планнеррецентпланреференце.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e27375e3f2395b3528873d8b83f0b5aa6f48d52e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583181"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>Тип ресурса Планнеррецентпланреференцеколлектион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **планнеррецентпланреференцеколлектион** представляет коллекцию ссылок на планы, которые были недавно просмотрены пользователем. Этот ресурс является открытым типом и является частью объекта [plannerUser](planneruser.md) . Имя свойства — это идентификатор соответствующего плана. Значение в параметре "свойство-значение" является объектом [планнеррецентпланреференце](plannerrecentplanreference.md) .
При добавлении новых ссылок в эту коллекцию самые старые записи будут удаляться автоматически, когда размер коллекции превышает предварительно заданное максимальное значение.


## <a name="properties"></a>Свойства
Вы можете определить свойства этого открытого типа. Имена свойств — это `id` значения ресурсов [plannerPlan](plannerplan.md) и их значения должны быть [планнеррецентпланреференце](plannerrecentplanreference.md) объектами. Чтобы удалить элемент из списка "Избранное", присвойте свойству значение `null`.


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
