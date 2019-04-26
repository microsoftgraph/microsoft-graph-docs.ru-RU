---
title: Тип ресурса Filter
description: Определяет, какие объекты должны быть подготовлены для приложения. Например, вам может потребоваться предоставить только пользователей, которые находятся в США. При наличии фильтра областей объекты, которые не соответствуют фильтру, будут пропущены во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 0aa75f3b3116991696e9456d7cdfc7b0f72ea86e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345590"
---
# <a name="filter-resource-type"></a><span data-ttu-id="fb223-105">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="fb223-105">filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb223-106">Определяет, какие объекты должны быть подготовлены для приложения.</span><span class="sxs-lookup"><span data-stu-id="fb223-106">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="fb223-107">Например, вам может потребоваться предоставить только пользователей, которые находятся в США.</span><span class="sxs-lookup"><span data-stu-id="fb223-107">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="fb223-108">При наличии фильтра областей объекты, которые не соответствуют фильтру, будут пропущены во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fb223-108">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="fb223-109">Фильтр является частью [сопоставления объектов](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="fb223-109">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="fb223-110">Он состоит из нескольких наборов групп фильтров, а каждая группа фильтра содержит одно или несколько предложений.</span><span class="sxs-lookup"><span data-stu-id="fb223-110">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="fb223-111">Объект рассматривается в области для группы (Группа оценивается как `true`) только в `true`том случае, если все предложения группы оцениваются.</span><span class="sxs-lookup"><span data-stu-id="fb223-111">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="fb223-112">Объект рассматривается в области для набора групп (набор групп оценивается как `true`), если для `true`каждой из групп в наборе вычислена значение.</span><span class="sxs-lookup"><span data-stu-id="fb223-112">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="fb223-113">Дополнительные сведения см в разделе [Подготовка приложений на основе атрибутов с помощью фильтров областей](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="fb223-113">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="fb223-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb223-114">Properties</span></span>
| <span data-ttu-id="fb223-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb223-115">Property</span></span>     | <span data-ttu-id="fb223-116">Тип</span><span class="sxs-lookup"><span data-stu-id="fb223-116">Type</span></span>   |<span data-ttu-id="fb223-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fb223-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb223-118">Категорифилтерграупс</span><span class="sxs-lookup"><span data-stu-id="fb223-118">categoryFilterGroups</span></span>|<span data-ttu-id="fb223-119">Коллекция [филтерграуп](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="fb223-119">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="fb223-120">`*Experimental*`Набор групп фильтров, используемый, чтобы определить, принадлежит ли данный объект и должен ли он обрабатываться как часть этого сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="fb223-120">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="fb223-121">Объект считается в области действия, \*Если любая из групп в коллекции оценивается как `true` \*.</span><span class="sxs-lookup"><span data-stu-id="fb223-121">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="fb223-122">groups</span><span class="sxs-lookup"><span data-stu-id="fb223-122">groups</span></span>|<span data-ttu-id="fb223-123">Коллекция [филтерграуп](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="fb223-123">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="fb223-124">Набор групп фильтров, используемый для определения того, находится ли заданный объект в области для подготовки.</span><span class="sxs-lookup"><span data-stu-id="fb223-124">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="fb223-125">**Это фильтр, который следует использовать в большинстве случаев**.</span><span class="sxs-lookup"><span data-stu-id="fb223-125">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="fb223-126">Если объект, используемый для выполнения этого фильтра, в данный момент, а затем объект или фильтр изменились так, что фильтр не удовлетворен более длинным, такой объект \* будет передано.</span><span class="sxs-lookup"><span data-stu-id="fb223-126">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="fb223-127">Объект считается в области действия, \*Если любая из групп в коллекции оценивается как `true` \*.</span><span class="sxs-lookup"><span data-stu-id="fb223-127">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="fb223-128">Инпутфилтерграупс</span><span class="sxs-lookup"><span data-stu-id="fb223-128">inputFilterGroups</span></span>|<span data-ttu-id="fb223-129">Коллекция [филтерграуп](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="fb223-129">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="fb223-130">`*Experimental*`Набор групп фильтров, используемый для фильтрации объектов на раннем этапе чтения их из каталога.</span><span class="sxs-lookup"><span data-stu-id="fb223-130">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="fb223-131">Если объект не соответствует этому фильтру, он не будет обрабатываться далее.</span><span class="sxs-lookup"><span data-stu-id="fb223-131">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="fb223-132">Важно понимать, что если объект, используемый для выполнения этого фильтра, в данный момент, а затем объект или фильтр изменился, так как фильтр больше не удовлетворен, такой объект *не*передается.</span><span class="sxs-lookup"><span data-stu-id="fb223-132">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="fb223-133">Объект считается в области действия, \*Если любая из групп в коллекции оценивается как `true` \*.</span><span class="sxs-lookup"><span data-stu-id="fb223-133">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fb223-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fb223-134">JSON representation</span></span>

<span data-ttu-id="fb223-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb223-135">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
