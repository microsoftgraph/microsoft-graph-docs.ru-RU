---
title: Тип ресурса Планнерпланконтекстколлектион
description: Ресурс **планнерпланконтекстколлектион** представляет коллекцию внешних контекстов, с которыми связан план. Этот ресурс является открытым типом и является частью объекта plannerPlan. Значение в параметре "свойство-значение" является объектом Планнерпланконтекст.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 45b09a0cca28a9efdc1a62b4d404d0966587fd9f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094941"
---
# <a name="plannerplancontextcollection-resource-type"></a>Тип ресурса Планнерпланконтекстколлектион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Ресурс **планнерпланконтекстколлектион** представляет коллекцию внешних контекстов, с которыми связан план. Этот ресурс является открытым типом и является частью объекта [plannerPlan](plannerplan.md) . Значение в параметре "свойство-значение" является объектом [планнерпланконтекст](plannerplancontext.md) .


## <a name="properties"></a>Свойства
Вы можете определить свойства этого открытого типа. Значения свойств должны представлять собой отличительный идентификатор, представляющий внешний контекст в качестве имени свойства. Значения свойств должны быть [планнерпланконтекст](plannerplancontext.md) объектами. В зависимости от требований OData имена свойств в открытых типах не могут содержать следующие символы: `.` , `:` , `%` , `@` . Эти символы необходимо закодировать с помощью URL-кодировки. Чтобы удалить элемент из списка "Избранное", присвойте свойству значение `null` .

## <a name="json-representation"></a>Представление в формате JSON

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


