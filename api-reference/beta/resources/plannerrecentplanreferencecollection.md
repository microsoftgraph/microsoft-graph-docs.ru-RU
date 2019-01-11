---
title: Тип ресурса plannerRecentPlanReferenceCollection
description: Ресурс **plannerRecentPlanReferenceCollection** представляет коллекцию ссылок на планы, которые были недавно просмотре пользователем. Этот ресурс является открытым и является частью объекта plannerUser. Имя свойства — это идентификатор соответствующего плана. Значение в паре значение свойства — это объект plannerRecentPlanReference.
localization_priority: Normal
ms.openlocfilehash: e77769cbe3a7e53dce518c73cd7c5228d1077dac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877345"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>Тип ресурса plannerRecentPlanReferenceCollection

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
