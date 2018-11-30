---
title: Тип ресурса plannerRecentPlanReferenceCollection
description: Ресурс **plannerRecentPlanReferenceCollection** представляет коллекцию ссылок на планы, которые были недавно просмотре пользователем. Этот ресурс является открытым и является частью объекта plannerUser. Имя свойства — это идентификатор соответствующего плана. Значение в паре значение свойства — это объект plannerRecentPlanReference.
ms.openlocfilehash: b22f7367a1826c95889b63a6884885ce49497c33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082663"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="9c83d-106">Тип ресурса plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="9c83d-106">plannerRecentPlanReferenceCollection resource type</span></span>

> <span data-ttu-id="9c83d-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c83d-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c83d-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c83d-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c83d-109">Ресурс **plannerRecentPlanReferenceCollection** представляет коллекцию ссылок на планы, которые были недавно просмотре пользователем.</span><span class="sxs-lookup"><span data-stu-id="9c83d-109">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="9c83d-110">Этот ресурс является открытым и является частью объекта [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="9c83d-110">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="9c83d-111">Имя свойства — это идентификатор соответствующего плана.</span><span class="sxs-lookup"><span data-stu-id="9c83d-111">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="9c83d-112">Значение в паре значение свойства — это объект [plannerRecentPlanReference](plannerrecentplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="9c83d-112">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="9c83d-113">Добавление новой ссылки для данного семейства сайтов автоматическое удаление старых записей, при превышении предопределенное значение максимального размера семейства.</span><span class="sxs-lookup"><span data-stu-id="9c83d-113">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="9c83d-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c83d-114">Properties</span></span>
<span data-ttu-id="9c83d-115">Можно определить свойства этого типа open.</span><span class="sxs-lookup"><span data-stu-id="9c83d-115">You can define the properties of this open type.</span></span> <span data-ttu-id="9c83d-116">Имена свойств являются `id` значений [plannerPlan](plannerplan.md) ресурсов и их значения должны быть [plannerRecentPlanReference](plannerrecentplanreference.md) объектов.</span><span class="sxs-lookup"><span data-stu-id="9c83d-116">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="9c83d-117">Чтобы удалить элемент в списке "Избранное", задайте значение свойства, которое должно `null`.</span><span class="sxs-lookup"><span data-stu-id="9c83d-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9c83d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c83d-118">JSON representation</span></span>

<span data-ttu-id="9c83d-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c83d-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
