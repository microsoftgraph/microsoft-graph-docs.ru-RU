---
title: Тип ресурса plannerFavoritePlanReferenceCollection
description: " значение — это объект plannerFavoritePlanReference."
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: 933589d455a683598576aa5c83df8bd19e6b553f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828443"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a>Тип ресурса plannerFavoritePlanReferenceCollection

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerFavoritePlanReferenceCollection** представляет коллекцию ссылок на планы, которые помечены как Избранное пользователя. Этот ресурс является открытым и является частью объекта [plannerUser](planneruser.md) . Имя свойства в паре значение свойства — это идентификатор соответствующего плана. значение — это объект [plannerFavoritePlanReference](plannerfavoriteplanreference.md) .


## <a name="properties"></a>Свойства
Можно определить свойства этого типа open. Имена свойств являются `id` значений [plannerPlan](plannerplan.md) ресурсов и их значения должны быть [plannerFavoritePlanReference](plannerfavoriteplanreference.md) объектов. Чтобы удалить элемент в списке "Избранное", задайте значение свойства, которое должно `null`.


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
}-->

```json
{
  "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586866870001551087",
    "planTitle": "Customer reviews"
  },
  "uZWtCtli30CGoWLIWSat1mQAC0ai": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586848705198093378",
    "planTitle": "Order Management (December 2017)"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
