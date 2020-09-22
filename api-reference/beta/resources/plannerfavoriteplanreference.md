---
title: Тип ресурса Планнерфаворитепланреференце
description: 'Тип ресурса **планнерфаворитепланреференце** репесентс ссылку на plannerPlan, помеченную пользователем в качестве избранного. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e5a25f7a1e4e27ca0d0061c616f441dd8cc53cde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979352"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="deaa1-103">Тип ресурса Планнерфаворитепланреференце</span><span class="sxs-lookup"><span data-stu-id="deaa1-103">plannerFavoritePlanReference resource type</span></span>

<span data-ttu-id="deaa1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deaa1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deaa1-105">Тип ресурса **планнерфаворитепланреференце** репесентс ссылку на [plannerPlan](plannerplan.md) , помеченную пользователем в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="deaa1-105">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="deaa1-106">Клиенты должны отметить, что записи **планнерфаворитепланреференце** могут ссылаться на **планов** , которые были удалены, что пользователь больше не может получить доступ, или он был обновлен с другим названием.</span><span class="sxs-lookup"><span data-stu-id="deaa1-106">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="deaa1-107">Мы рекомендуем клиентам уведомлять пользователей о наличии расхождений и постоянном обновлении записей.</span><span class="sxs-lookup"><span data-stu-id="deaa1-107">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="deaa1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="deaa1-108">Properties</span></span>
| <span data-ttu-id="deaa1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="deaa1-109">Property</span></span>     | <span data-ttu-id="deaa1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="deaa1-110">Type</span></span>   |<span data-ttu-id="deaa1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="deaa1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deaa1-112">orderHint</span><span class="sxs-lookup"><span data-stu-id="deaa1-112">orderHint</span></span>|<span data-ttu-id="deaa1-113">String</span><span class="sxs-lookup"><span data-stu-id="deaa1-113">String</span></span>|<span data-ttu-id="deaa1-p102">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="deaa1-p102">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="deaa1-116">плантитле</span><span class="sxs-lookup"><span data-stu-id="deaa1-116">planTitle</span></span>|<span data-ttu-id="deaa1-117">String</span><span class="sxs-lookup"><span data-stu-id="deaa1-117">String</span></span>|<span data-ttu-id="deaa1-118">Название плана на тот момент, когда пользователь пометил его в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="deaa1-118">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="deaa1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="deaa1-119">JSON representation</span></span>

<span data-ttu-id="deaa1-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="deaa1-120">The following is a JSON representation of the resource.</span></span>

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


