---
title: Тип ресурса plannerFavoritePlanReferenceCollection
description: " значение — это объект plannerFavoritePlanReference."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 333d7f354f056945de52687eefc8bb862ac48e75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967114"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="7b8f3-103">Тип ресурса plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="7b8f3-103">plannerFavoritePlanReferenceCollection resource type</span></span>

> <span data-ttu-id="7b8f3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b8f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b8f3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b8f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b8f3-106">Ресурс **plannerFavoritePlanReferenceCollection** представляет коллекцию ссылок на планы, которые помечены как Избранное пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b8f3-106">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="7b8f3-107">Этот ресурс является открытым и является частью объекта [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="7b8f3-107">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="7b8f3-108">Имя свойства в паре значение свойства — это идентификатор соответствующего плана. значение — это объект [plannerFavoritePlanReference](plannerfavoriteplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="7b8f3-108">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="7b8f3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b8f3-109">Properties</span></span>
<span data-ttu-id="7b8f3-110">Можно определить свойства этого типа open.</span><span class="sxs-lookup"><span data-stu-id="7b8f3-110">You can define the properties of this open type.</span></span> <span data-ttu-id="7b8f3-111">Имена свойств являются `id` значений [plannerPlan](plannerplan.md) ресурсов и их значения должны быть [plannerFavoritePlanReference](plannerfavoriteplanreference.md) объектов.</span><span class="sxs-lookup"><span data-stu-id="7b8f3-111">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="7b8f3-112">Чтобы удалить элемент в списке "Избранное", задайте значение свойства, которое должно `null`.</span><span class="sxs-lookup"><span data-stu-id="7b8f3-112">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7b8f3-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b8f3-113">JSON representation</span></span>

<span data-ttu-id="7b8f3-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b8f3-114">The following is a JSON representation of the resource.</span></span>

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
