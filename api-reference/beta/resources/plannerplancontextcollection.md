---
title: тип ресурса plannerPlanContextCollection
description: Ресурс **plannerPlanContextCollection** представляет коллекцию внешних контекстов, к которым связан план. Этот ресурс является открытым типом и является частью объекта plannerPlan. Значение в паре свойство-значение — объект plannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b2069fd30ba3beb6150b0fdc5dd5bb0f69956b82
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473600"
---
# <a name="plannerplancontextcollection-resource-type"></a>тип ресурса plannerPlanContextCollection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Ресурс **plannerPlanContextCollection** представляет коллекцию внешних контекстов, к которым связан план. Этот ресурс является открытым типом и является частью [объекта plannerPlan.](plannerplan.md) Значение в паре свойство-значение — объект [plannerPlanContext.](plannerplancontext.md)


## <a name="properties"></a>Свойства
Можно определить свойства этого открытого типа. Значения свойств должны быть отличительными идентификаторами, представляюми внешний контекст в качестве имени свойства. Значения свойств должны быть [объектами plannerPlanContext.](plannerplancontext.md) На основании требований OData имена свойств в открытых типах не могут содержать следующие символы: `.` , , , , `:` `%` `@` `#` . Эти символы необходимо кодировать с помощью кодирования URL-адресов. Чтобы удалить элемент в списке избранного, установите значение свойства `null` .

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


