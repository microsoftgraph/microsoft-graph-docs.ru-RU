---
title: Тип ресурса Планнерфаворитепланреференцеколлектион
description: " значение — объект Планнерфаворитепланреференце."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 67149f0ccf8ec04fe702a0d77b1fb2f5f6020365
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965952"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="28bcb-103">Тип ресурса Планнерфаворитепланреференцеколлектион</span><span class="sxs-lookup"><span data-stu-id="28bcb-103">plannerFavoritePlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28bcb-104">Ресурс **планнерфаворитепланреференцеколлектион** представляет коллекцию ссылок на планы, помеченные пользователем в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="28bcb-104">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="28bcb-105">Этот ресурс является открытым типом и является частью объекта [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="28bcb-105">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="28bcb-106">Имя свойства в разделе "свойство-значение" является ИДЕНТИФИКАТОРом соответствующего плана; значение — объект [планнерфаворитепланреференце](plannerfavoriteplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="28bcb-106">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="28bcb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="28bcb-107">Properties</span></span>
<span data-ttu-id="28bcb-108">Вы можете определить свойства этого открытого типа.</span><span class="sxs-lookup"><span data-stu-id="28bcb-108">You can define the properties of this open type.</span></span> <span data-ttu-id="28bcb-109">Имена свойств — это `id` значения ресурсов [plannerPlan](plannerplan.md) и их значения должны быть [планнерфаворитепланреференце](plannerfavoriteplanreference.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="28bcb-109">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="28bcb-110">Чтобы удалить элемент из списка "Избранное", присвойте свойству значение `null`.</span><span class="sxs-lookup"><span data-stu-id="28bcb-110">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="28bcb-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28bcb-111">JSON representation</span></span>

<span data-ttu-id="28bcb-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28bcb-112">The following is a JSON representation of the resource.</span></span>

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
