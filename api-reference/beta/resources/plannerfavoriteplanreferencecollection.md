---
title: Тип ресурса Планнерфаворитепланреференцеколлектион
description: " значение — объект Планнерфаворитепланреференце."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 32c0cecc402570491c0025c0b4e0c88b74ed40fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521736"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="4116b-103">Тип ресурса Планнерфаворитепланреференцеколлектион</span><span class="sxs-lookup"><span data-stu-id="4116b-103">plannerFavoritePlanReferenceCollection resource type</span></span>

<span data-ttu-id="4116b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4116b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4116b-105">Ресурс **планнерфаворитепланреференцеколлектион** представляет коллекцию ссылок на планы, помеченные пользователем в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="4116b-105">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="4116b-106">Этот ресурс является открытым типом и является частью объекта [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="4116b-106">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="4116b-107">Имя свойства в разделе "свойство-значение" является ИДЕНТИФИКАТОРом соответствующего плана; значение — объект [планнерфаворитепланреференце](plannerfavoriteplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="4116b-107">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="4116b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4116b-108">Properties</span></span>
<span data-ttu-id="4116b-109">Вы можете определить свойства этого открытого типа.</span><span class="sxs-lookup"><span data-stu-id="4116b-109">You can define the properties of this open type.</span></span> <span data-ttu-id="4116b-110">Имена свойств — это `id` значения ресурсов [plannerPlan](plannerplan.md) и их значения должны быть [планнерфаворитепланреференце](plannerfavoriteplanreference.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="4116b-110">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="4116b-111">Чтобы удалить элемент из списка "Избранное", присвойте свойству значение `null`.</span><span class="sxs-lookup"><span data-stu-id="4116b-111">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4116b-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4116b-112">JSON representation</span></span>

<span data-ttu-id="4116b-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4116b-113">The following is a JSON representation of the resource.</span></span>

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
