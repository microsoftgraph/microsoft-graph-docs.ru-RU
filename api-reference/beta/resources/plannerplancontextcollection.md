---
title: Тип ресурса plannerPlanContextCollection
description: Ресурс **plannerPlanContextCollection** представляет коллекцию внешних контекстах, с которыми связан плана. Этот ресурс является открытым и является частью объекта plannerPlan. Значение в паре значение свойства — это объект plannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6ec515a164c5b0fca6334930b55a4b5d4e73b7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516499"
---
# <a name="plannerplancontextcollection-resource-type"></a>Тип ресурса plannerPlanContextCollection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextcollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
