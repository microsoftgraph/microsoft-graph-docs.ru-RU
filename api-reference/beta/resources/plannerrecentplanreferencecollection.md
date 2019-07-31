---
title: Тип ресурса Планнеррецентпланреференцеколлектион
description: Ресурс **планнеррецентпланреференцеколлектион** представляет коллекцию ссылок на планы, которые были недавно просмотрены пользователем. Этот ресурс является открытым типом и является частью объекта plannerUser. Имя свойства — это идентификатор соответствующего плана. Значение в параметре "свойство-значение" является объектом Планнеррецентпланреференце.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 474cd321357e698d65b768b94fb867285978984b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965861"
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
  "suppressions": []
}
-->
