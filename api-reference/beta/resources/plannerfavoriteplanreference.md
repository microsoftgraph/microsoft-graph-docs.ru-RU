---
title: Тип ресурса plannerFavoritePlanReference
description: 'Repesents тип **plannerFavoritePlanReference** ресурсов ссылку на plannerPlan, который был помечен как Избранное пользователя. '
localization_priority: Normal
ms.openlocfilehash: b17846eaa1b9a9859d23735d18a191cae4872542
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871325"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="b72fc-103">Тип ресурса plannerFavoritePlanReference</span><span class="sxs-lookup"><span data-stu-id="b72fc-103">plannerFavoritePlanReference resource type</span></span>

> <span data-ttu-id="b72fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b72fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b72fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b72fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b72fc-106">Repesents тип **plannerFavoritePlanReference** ресурсов ссылку на [plannerPlan](plannerplan.md) , который был помечен как Избранное пользователя.</span><span class="sxs-lookup"><span data-stu-id="b72fc-106">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="b72fc-107">Клиенты следует иметь в виду, что записи **plannerFavoritePlanReference** можно ссылаться на **plannerPlans** , будут удалены, пользователь больше не может получить доступ и добавлены иное название.</span><span class="sxs-lookup"><span data-stu-id="b72fc-107">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="b72fc-108">Рекомендуется уведомлять пользователей есть несоответствия клиентов и обновлять записи.</span><span class="sxs-lookup"><span data-stu-id="b72fc-108">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="b72fc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b72fc-109">Properties</span></span>
| <span data-ttu-id="b72fc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b72fc-110">Property</span></span>     | <span data-ttu-id="b72fc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b72fc-111">Type</span></span>   |<span data-ttu-id="b72fc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b72fc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b72fc-113">orderHint</span><span class="sxs-lookup"><span data-stu-id="b72fc-113">orderHint</span></span>|<span data-ttu-id="b72fc-114">Строка</span><span class="sxs-lookup"><span data-stu-id="b72fc-114">String</span></span>|<span data-ttu-id="b72fc-p103">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="b72fc-p103">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="b72fc-117">planTitle</span><span class="sxs-lookup"><span data-stu-id="b72fc-117">planTitle</span></span>|<span data-ttu-id="b72fc-118">Строка</span><span class="sxs-lookup"><span data-stu-id="b72fc-118">String</span></span>|<span data-ttu-id="b72fc-119">Название плана в то время, что пользователь отметил его в список избранного.</span><span class="sxs-lookup"><span data-stu-id="b72fc-119">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b72fc-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b72fc-120">JSON representation</span></span>

<span data-ttu-id="b72fc-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b72fc-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
