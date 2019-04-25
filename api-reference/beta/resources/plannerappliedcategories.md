---
title: Тип ресурса Планнерапплиедкатегориес
description: Ресурс **апплиедкатегориесколлектион** представляет коллекцию категорий (или меток), которые были применены к задаче. Он является частью объекта plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b4e3ae92d179669d449d33c34ade4ae4476570fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541355"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="eee73-104">Тип ресурса Планнерапплиедкатегориес</span><span class="sxs-lookup"><span data-stu-id="eee73-104">plannerAppliedCategories resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eee73-105">Ресурс **апплиедкатегориесколлектион** представляет коллекцию категорий (или меток), которые были применены к задаче.</span><span class="sxs-lookup"><span data-stu-id="eee73-105">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task.</span></span> <span data-ttu-id="eee73-106">Он является частью объекта [plannerTask](plannertask.md) .</span><span class="sxs-lookup"><span data-stu-id="eee73-106">It is part of the [plannerTask](plannertask.md) object.</span></span>
<span data-ttu-id="eee73-107">К задаче может быть применено до 6 категорий.</span><span class="sxs-lookup"><span data-stu-id="eee73-107">There can be up to 6 categories applied to a task.</span></span> <span data-ttu-id="eee73-108">Описания категорий, например `category1`, `category2` и т. д., входят в состав объекта " [сведения о плане](plannerplandetails.md) ".</span><span class="sxs-lookup"><span data-stu-id="eee73-108">Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="eee73-109">Это открытый тип.</span><span class="sxs-lookup"><span data-stu-id="eee73-109">This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="eee73-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="eee73-110">Properties</span></span>
<span data-ttu-id="eee73-111">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="eee73-111">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="eee73-112">`category1`В этом случае клиент должен предоставлять, `category2`, `category3` `category4`, `category5` и/или `category6` как свойства со своими значениями `true` Boolean при применении соответствующих категорий к задаче.</span><span class="sxs-lookup"><span data-stu-id="eee73-112">In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task.</span></span> <span data-ttu-id="eee73-113">Пример показан ниже.</span><span class="sxs-lookup"><span data-stu-id="eee73-113">Example is shown below.</span></span> <span data-ttu-id="eee73-114">Если они не применяются, свойства автоматически удаляются путем присвоения их значений `false` логическому значению.</span><span class="sxs-lookup"><span data-stu-id="eee73-114">When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="eee73-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eee73-115">JSON representation</span></span>

<span data-ttu-id="eee73-116">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eee73-116">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="eee73-117">Пример.</span><span class="sxs-lookup"><span data-stu-id="eee73-117">Example:</span></span> 

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerappliedcategories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
