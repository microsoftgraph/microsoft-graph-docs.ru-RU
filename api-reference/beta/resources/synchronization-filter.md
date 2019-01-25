---
title: Тип ресурса Filter
description: Определяет, какие объекты, следует подготовить к приложению. Например может потребоваться только подготовки пользователей, которые расположены в США. Если фильтр области видимости, объекты, которые не удовлетворяют фильтра будет пропущено во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: acc9f2efcfeef68ee3beda7dc720b5da5dea2b1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516681"
---
# <a name="filter-resource-type"></a><span data-ttu-id="81a85-105">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="81a85-105">filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81a85-106">Определяет, какие объекты, следует подготовить к приложению.</span><span class="sxs-lookup"><span data-stu-id="81a85-106">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="81a85-107">Например может потребоваться только подготовки пользователей, которые расположены в США.</span><span class="sxs-lookup"><span data-stu-id="81a85-107">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="81a85-108">Если фильтр области видимости, объекты, которые не удовлетворяют фильтра будет пропущено во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="81a85-108">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="81a85-109">Фильтр является частью [сопоставление объектов](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="81a85-109">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="81a85-110">Состоит из нескольких наборов групп фильтра, и каждой группе фильтра содержит одно или несколько предложений.</span><span class="sxs-lookup"><span data-stu-id="81a85-110">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="81a85-111">Объект считается в области действия группы (рассчитано группы для `true`) только в том случае, если все предложения группе вычисляются для `true`.</span><span class="sxs-lookup"><span data-stu-id="81a85-111">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="81a85-112">Объект считается в области действия для набора группы (набор групп вычисляется для `true`) Если какие-либо группы в наборе оценивается `true`.</span><span class="sxs-lookup"><span data-stu-id="81a85-112">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="81a85-113">Для получения дополнительных сведений см. [Подготовка с помощью области видимости фильтры приложения на основе атрибутов](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="81a85-113">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="81a85-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="81a85-114">Properties</span></span>
| <span data-ttu-id="81a85-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="81a85-115">Property</span></span>     | <span data-ttu-id="81a85-116">Тип</span><span class="sxs-lookup"><span data-stu-id="81a85-116">Type</span></span>   |<span data-ttu-id="81a85-117">Описание</span><span class="sxs-lookup"><span data-stu-id="81a85-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81a85-118">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="81a85-118">categoryFilterGroups</span></span>|<span data-ttu-id="81a85-119">[filterGroup](synchronization-filtergroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81a85-119">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="81a85-120">`*Experimental*`Используются для определения, является ли указанный объект принадлежит группе установлен фильтр и будут обрабатываться как часть этого сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="81a85-120">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="81a85-121">Объект считается в области \*Если какие-либо группы в коллекции оценивается `true` \*.</span><span class="sxs-lookup"><span data-stu-id="81a85-121">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="81a85-122">группы</span><span class="sxs-lookup"><span data-stu-id="81a85-122">groups</span></span>|<span data-ttu-id="81a85-123">[filterGroup](synchronization-filtergroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81a85-123">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="81a85-124">Фильтровать набор группы, используемый в том, является ли указанный объект в области действия для подготовки.</span><span class="sxs-lookup"><span data-stu-id="81a85-124">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="81a85-125">**Это фильтр, который должен использоваться в большинстве случаев**.</span><span class="sxs-lookup"><span data-stu-id="81a85-125">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="81a85-126">Объект, используемый для удовлетворения этот фильтр в данный момент и затем объект или фильтр был изменен, поэтому этот фильтр не больше, удовлетворены такого объекта \* будет получить отзыва подготовить к работе».</span><span class="sxs-lookup"><span data-stu-id="81a85-126">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="81a85-127">Объект считается в области \*Если какие-либо группы в коллекции оценивается `true` \*.</span><span class="sxs-lookup"><span data-stu-id="81a85-127">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="81a85-128">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="81a85-128">inputFilterGroups</span></span>|<span data-ttu-id="81a85-129">[filterGroup](synchronization-filtergroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81a85-129">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="81a85-130">`*Experimental*`Фильтровать набор группы, используемый для фильтрации объектов на ранней стадии чтения их из каталога.</span><span class="sxs-lookup"><span data-stu-id="81a85-130">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="81a85-131">Если объект не удовлетворяют этот фильтр, которые не будут обрабатываться Дополнительно.</span><span class="sxs-lookup"><span data-stu-id="81a85-131">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="81a85-132">Важно понимать, что если объект используются для удовлетворения этот фильтр в данный момент, а затем объект или фильтр изменен, этот фильтр больше не выполняется, например объекта *будет не получите отзыва подготовить к работе*.</span><span class="sxs-lookup"><span data-stu-id="81a85-132">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="81a85-133">Объект считается в области \*Если какие-либо группы в коллекции оценивается `true` \*.</span><span class="sxs-lookup"><span data-stu-id="81a85-133">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81a85-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81a85-134">JSON representation</span></span>

<span data-ttu-id="81a85-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81a85-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
