---
title: Тип ресурса Планнерфаворитепланреференце
description: 'Тип ресурса **планнерфаворитепланреференце** репесентс ссылку на plannerPlan, помеченную пользователем в качестве избранного. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 07803375ca31162f0f7e392d81edb83ab2bd6da3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009071"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="f9e80-103">Тип ресурса Планнерфаворитепланреференце</span><span class="sxs-lookup"><span data-stu-id="f9e80-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9e80-104">Тип ресурса **планнерфаворитепланреференце** репесентс ссылку на [plannerPlan](plannerplan.md) , помеченную пользователем в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="f9e80-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="f9e80-105">Клиенты должны отметить, что записи **планнерфаворитепланреференце** могут ссылаться на **планов** , которые были удалены, что пользователь больше не может получить доступ, или он был обновлен с другим названием.</span><span class="sxs-lookup"><span data-stu-id="f9e80-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="f9e80-106">Мы рекомендуем клиентам уведомлять пользователей о наличии расхождений и постоянном обновлении записей.</span><span class="sxs-lookup"><span data-stu-id="f9e80-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="f9e80-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9e80-107">Properties</span></span>
| <span data-ttu-id="f9e80-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9e80-108">Property</span></span>     | <span data-ttu-id="f9e80-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f9e80-109">Type</span></span>   |<span data-ttu-id="f9e80-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f9e80-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9e80-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="f9e80-111">orderHint</span></span>|<span data-ttu-id="f9e80-112">String</span><span class="sxs-lookup"><span data-stu-id="f9e80-112">String</span></span>|<span data-ttu-id="f9e80-p102">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="f9e80-p102">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="f9e80-115">Плантитле</span><span class="sxs-lookup"><span data-stu-id="f9e80-115">planTitle</span></span>|<span data-ttu-id="f9e80-116">String</span><span class="sxs-lookup"><span data-stu-id="f9e80-116">String</span></span>|<span data-ttu-id="f9e80-117">Название плана на тот момент, когда пользователь пометил его в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="f9e80-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f9e80-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9e80-118">JSON representation</span></span>

<span data-ttu-id="f9e80-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9e80-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
