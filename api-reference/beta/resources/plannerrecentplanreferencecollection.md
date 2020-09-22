---
title: Тип ресурса Планнеррецентпланреференцеколлектион
description: Ресурс **планнеррецентпланреференцеколлектион** представляет коллекцию ссылок на планы, которые были недавно просмотрены пользователем. Этот ресурс является открытым типом и является частью объекта plannerUser. Имя свойства — это идентификатор соответствующего плана. Значение в параметре "свойство-значение" является объектом Планнеррецентпланреференце.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 529552be4497729824ddfb9fa9e84ea82e8ccd0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064019"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="2828f-106">Тип ресурса Планнеррецентпланреференцеколлектион</span><span class="sxs-lookup"><span data-stu-id="2828f-106">plannerRecentPlanReferenceCollection resource type</span></span>

<span data-ttu-id="2828f-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2828f-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2828f-108">Ресурс **планнеррецентпланреференцеколлектион** представляет коллекцию ссылок на планы, которые были недавно просмотрены пользователем.</span><span class="sxs-lookup"><span data-stu-id="2828f-108">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="2828f-109">Этот ресурс является открытым типом и является частью объекта [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="2828f-109">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="2828f-110">Имя свойства — это идентификатор соответствующего плана.</span><span class="sxs-lookup"><span data-stu-id="2828f-110">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="2828f-111">Значение в параметре "свойство-значение" является объектом [планнеррецентпланреференце](plannerrecentplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="2828f-111">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="2828f-112">При добавлении новых ссылок в эту коллекцию самые старые записи будут удаляться автоматически, когда размер коллекции превышает предварительно заданное максимальное значение.</span><span class="sxs-lookup"><span data-stu-id="2828f-112">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="2828f-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="2828f-113">Properties</span></span>
<span data-ttu-id="2828f-114">Вы можете определить свойства этого открытого типа.</span><span class="sxs-lookup"><span data-stu-id="2828f-114">You can define the properties of this open type.</span></span> <span data-ttu-id="2828f-115">Имена свойств — это `id` значения ресурсов [plannerPlan](plannerplan.md) и их значения должны быть [планнеррецентпланреференце](plannerrecentplanreference.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="2828f-115">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="2828f-116">Чтобы удалить элемент из списка "Избранное", присвойте свойству значение `null` .</span><span class="sxs-lookup"><span data-stu-id="2828f-116">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2828f-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2828f-117">JSON representation</span></span>

<span data-ttu-id="2828f-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2828f-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


