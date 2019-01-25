---
title: Тип ресурса filterGroup
description: Определяет набор условий, которые должны соответствовать объекта следует учитывать в области. Объект считается в области действия группы (рассчитано группы для `true`) только в том случае, если все предложения группе вычисляются для `true`.
localization_priority: Normal
ms.openlocfilehash: b71bdf16d6639b5ecc8512565ccf56d592a0da58
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514189"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="6fc03-104">Тип ресурса filterGroup</span><span class="sxs-lookup"><span data-stu-id="6fc03-104">filterGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fc03-105">Определяет набор условий, которые должны соответствовать объекта следует учитывать в области.</span><span class="sxs-lookup"><span data-stu-id="6fc03-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="6fc03-106">Объект считается в области действия группы (рассчитано группы для `true`) только в том случае, если все предложения группе вычисляются для `true`.</span><span class="sxs-lookup"><span data-stu-id="6fc03-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="6fc03-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fc03-107">Properties</span></span>
| <span data-ttu-id="6fc03-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fc03-108">Property</span></span>     | <span data-ttu-id="6fc03-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6fc03-109">Type</span></span>   |<span data-ttu-id="6fc03-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6fc03-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fc03-111">Предложения</span><span class="sxs-lookup"><span data-stu-id="6fc03-111">clauses</span></span>|<span data-ttu-id="6fc03-112">[filterClause](synchronization-filterclause.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6fc03-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="6fc03-113">Фильтрация условия (условия) этой группы.</span><span class="sxs-lookup"><span data-stu-id="6fc03-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="6fc03-114">Все предложения в группе должны быть выполнены в порядке для группы фильтра для вычисления `true`.</span><span class="sxs-lookup"><span data-stu-id="6fc03-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="6fc03-115">name</span><span class="sxs-lookup"><span data-stu-id="6fc03-115">name</span></span>|<span data-ttu-id="6fc03-116">String</span><span class="sxs-lookup"><span data-stu-id="6fc03-116">String</span></span>|<span data-ttu-id="6fc03-117">Понятное имя группы фильтра.</span><span class="sxs-lookup"><span data-stu-id="6fc03-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fc03-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fc03-118">JSON representation</span></span>

<span data-ttu-id="6fc03-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fc03-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filtergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
