---
title: Тип ресурса plannerPlanContextCollection
description: Ресурс **plannerPlanContextCollection** представляет коллекцию внешних контекстах, с которыми связан плана. Этот ресурс является открытым и является частью объекта plannerPlan. Значение в паре значение свойства — это объект plannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 3281a7664561ac32c3908ca059209a1b89b4ea7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951812"
---
# <a name="plannerplancontextcollection-resource-type"></a>Тип ресурса plannerPlanContextCollection

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.


Ресурс **plannerPlanContextCollection** представляет коллекцию внешних контекстах, с которыми связан плана. Этот ресурс является открытым и является частью объекта [plannerPlan](plannerplan.md) . Значение в паре значение свойства — это объект [plannerPlanContext](plannerplancontext.md) .


## <a name="properties"></a>Свойства
Можно определить свойства этого типа open. Значения свойства должны быть особый идентификатор, представляющий внешнего контекста как имя свойства. Значения свойства должны быть [plannerPlanContext](plannerplancontext.md) объектов. На основании требований к OData, имена свойств в открытые типы не может содержать следующие символы: `.`, `:`, `%`, `@`. Эти символы должны быть закодированы с помощью Кодировка URL-адрес. Чтобы удалить элемент в списке "Избранное", задайте значение свойства, которое должно `null`.

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
