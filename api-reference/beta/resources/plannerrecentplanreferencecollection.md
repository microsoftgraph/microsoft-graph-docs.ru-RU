---
title: Тип ресурса Планнеррецентпланреференцеколлектион
description: Ресурс **планнеррецентпланреференцеколлектион** представляет коллекцию ссылок на планы, которые были недавно просмотрены пользователем. Этот ресурс является открытым типом и является частью объекта plannerUser. Имя свойства — это идентификатор соответствующего плана. Значение в параметре "свойство-значение" является объектом Планнеррецентпланреференце.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e27375e3f2395b3528873d8b83f0b5aa6f48d52e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583181"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="a4df8-106">Тип ресурса Планнеррецентпланреференцеколлектион</span><span class="sxs-lookup"><span data-stu-id="a4df8-106">plannerRecentPlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4df8-107">Ресурс **планнеррецентпланреференцеколлектион** представляет коллекцию ссылок на планы, которые были недавно просмотрены пользователем.</span><span class="sxs-lookup"><span data-stu-id="a4df8-107">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="a4df8-108">Этот ресурс является открытым типом и является частью объекта [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="a4df8-108">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="a4df8-109">Имя свойства — это идентификатор соответствующего плана.</span><span class="sxs-lookup"><span data-stu-id="a4df8-109">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="a4df8-110">Значение в параметре "свойство-значение" является объектом [планнеррецентпланреференце](plannerrecentplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="a4df8-110">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="a4df8-111">При добавлении новых ссылок в эту коллекцию самые старые записи будут удаляться автоматически, когда размер коллекции превышает предварительно заданное максимальное значение.</span><span class="sxs-lookup"><span data-stu-id="a4df8-111">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="a4df8-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4df8-112">Properties</span></span>
<span data-ttu-id="a4df8-113">Вы можете определить свойства этого открытого типа.</span><span class="sxs-lookup"><span data-stu-id="a4df8-113">You can define the properties of this open type.</span></span> <span data-ttu-id="a4df8-114">Имена свойств — это `id` значения ресурсов [plannerPlan](plannerplan.md) и их значения должны быть [планнеррецентпланреференце](plannerrecentplanreference.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="a4df8-114">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="a4df8-115">Чтобы удалить элемент из списка "Избранное", присвойте свойству значение `null`.</span><span class="sxs-lookup"><span data-stu-id="a4df8-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a4df8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4df8-116">JSON representation</span></span>

<span data-ttu-id="a4df8-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4df8-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
