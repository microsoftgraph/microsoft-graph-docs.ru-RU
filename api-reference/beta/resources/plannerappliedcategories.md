---
title: Тип ресурса Планнерапплиедкатегориес
description: Ресурс **апплиедкатегориесколлектион** представляет коллекцию категорий (или меток), которые были применены к задаче. Он является частью объекта plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: bacf2ed499d420006173af8b3616a14b7c487904
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521820"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="e4f68-104">Тип ресурса Планнерапплиедкатегориес</span><span class="sxs-lookup"><span data-stu-id="e4f68-104">plannerAppliedCategories resource type</span></span>

<span data-ttu-id="e4f68-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e4f68-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f68-106">Ресурс **апплиедкатегориесколлектион** представляет коллекцию категорий (или меток), которые были применены к задаче.</span><span class="sxs-lookup"><span data-stu-id="e4f68-106">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task.</span></span> <span data-ttu-id="e4f68-107">Он является частью объекта [plannerTask](plannertask.md) .</span><span class="sxs-lookup"><span data-stu-id="e4f68-107">It is part of the [plannerTask](plannertask.md) object.</span></span>
<span data-ttu-id="e4f68-108">К задаче может быть применено до 6 категорий.</span><span class="sxs-lookup"><span data-stu-id="e4f68-108">There can be up to 6 categories applied to a task.</span></span> <span data-ttu-id="e4f68-109">Описания категорий, например `category1`, `category2` и т. д., входят в состав объекта " [сведения о плане](plannerplandetails.md) ".</span><span class="sxs-lookup"><span data-stu-id="e4f68-109">Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="e4f68-110">Это открытый тип.</span><span class="sxs-lookup"><span data-stu-id="e4f68-110">This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="e4f68-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4f68-111">Properties</span></span>
<span data-ttu-id="e4f68-112">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="e4f68-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="e4f68-113">`category1`В этом случае клиент должен предоставлять, `category2`, `category3` `category4`, `category5` и/или `category6` как свойства со своими значениями `true` Boolean при применении соответствующих категорий к задаче.</span><span class="sxs-lookup"><span data-stu-id="e4f68-113">In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task.</span></span> <span data-ttu-id="e4f68-114">Пример показан ниже.</span><span class="sxs-lookup"><span data-stu-id="e4f68-114">Example is shown below.</span></span> <span data-ttu-id="e4f68-115">Если они не применяются, свойства автоматически удаляются путем присвоения их значений `false` логическому значению.</span><span class="sxs-lookup"><span data-stu-id="e4f68-115">When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="e4f68-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4f68-116">JSON representation</span></span>

<span data-ttu-id="e4f68-117">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e4f68-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="e4f68-118">Пример.</span><span class="sxs-lookup"><span data-stu-id="e4f68-118">Example:</span></span> 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
