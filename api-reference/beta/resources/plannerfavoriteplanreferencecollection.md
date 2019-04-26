---
title: Тип ресурса Планнерфаворитепланреференцеколлектион
description: " значение — объект Планнерфаворитепланреференце."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 8c43108ed5c9e2f27b824d772716c6e467d56942
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344522"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a>Тип ресурса Планнерфаворитепланреференцеколлектион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **планнерфаворитепланреференцеколлектион** представляет коллекцию ссылок на планы, помеченные пользователем в качестве избранного. Этот ресурс является открытым типом и является частью объекта [plannerUser](planneruser.md) . Имя свойства в разделе "свойство-значение" является ИДЕНТИФИКАТОРом соответствующего плана; значение — объект [планнерфаворитепланреференце](plannerfavoriteplanreference.md) .


## <a name="properties"></a>Свойства
Вы можете определить свойства этого открытого типа. Имена свойств — это `id` значения ресурсов [plannerPlan](plannerplan.md) и их значения должны быть [планнерфаворитепланреференце](plannerfavoriteplanreference.md) объектами. Чтобы удалить элемент из списка "Избранное", присвойте свойству значение `null`.


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
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
