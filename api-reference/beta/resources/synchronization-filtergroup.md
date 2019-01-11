---
title: Тип ресурса filterGroup
description: Определяет набор условий, которые должны соответствовать объекта следует учитывать в области. Объект считается в области действия группы (рассчитано группы для `true`) только в том случае, если все предложения группе вычисляются для `true`.
localization_priority: Normal
ms.openlocfilehash: 174c02518069e949c49887d9e21e778e8455509a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836115"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="7b326-104">Тип ресурса filterGroup</span><span class="sxs-lookup"><span data-stu-id="7b326-104">filterGroup resource type</span></span>

> <span data-ttu-id="7b326-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b326-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b326-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b326-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b326-107">Определяет набор условий, которые должны соответствовать объекта следует учитывать в области.</span><span class="sxs-lookup"><span data-stu-id="7b326-107">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="7b326-108">Объект считается в области действия группы (рассчитано группы для `true`) только в том случае, если все предложения группе вычисляются для `true`.</span><span class="sxs-lookup"><span data-stu-id="7b326-108">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="7b326-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b326-109">Properties</span></span>
| <span data-ttu-id="7b326-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b326-110">Property</span></span>     | <span data-ttu-id="7b326-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7b326-111">Type</span></span>   |<span data-ttu-id="7b326-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7b326-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b326-113">предложения</span><span class="sxs-lookup"><span data-stu-id="7b326-113">clauses</span></span>|<span data-ttu-id="7b326-114">[filterClause](synchronization-filterclause.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7b326-114">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="7b326-115">Фильтрация условия (условия) этой группы.</span><span class="sxs-lookup"><span data-stu-id="7b326-115">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="7b326-116">Все предложения в группе должны быть выполнены в порядке для группы фильтра для вычисления `true`.</span><span class="sxs-lookup"><span data-stu-id="7b326-116">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="7b326-117">name</span><span class="sxs-lookup"><span data-stu-id="7b326-117">name</span></span>|<span data-ttu-id="7b326-118">Строка</span><span class="sxs-lookup"><span data-stu-id="7b326-118">String</span></span>|<span data-ttu-id="7b326-119">Понятное имя группы фильтра.</span><span class="sxs-lookup"><span data-stu-id="7b326-119">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b326-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b326-120">JSON representation</span></span>

<span data-ttu-id="7b326-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b326-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
