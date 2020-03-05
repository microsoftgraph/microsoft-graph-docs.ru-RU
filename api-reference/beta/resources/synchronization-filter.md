---
title: Тип ресурса Filter
description: Определяет, какие объекты должны быть подготовлены для приложения. Например, вам может потребоваться предоставить только пользователей, которые находятся в США. При наличии фильтра областей объекты, которые не соответствуют фильтру, будут пропущены во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9e7e4cfc629cb8586c1fd1cf2e32474b0bc6b6cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520200"
---
# <a name="filter-resource-type"></a><span data-ttu-id="09823-105">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="09823-105">filter resource type</span></span>

<span data-ttu-id="09823-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="09823-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09823-107">Определяет, какие объекты должны быть подготовлены для приложения.</span><span class="sxs-lookup"><span data-stu-id="09823-107">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="09823-108">Например, вам может потребоваться предоставить только пользователей, которые находятся в США.</span><span class="sxs-lookup"><span data-stu-id="09823-108">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="09823-109">При наличии фильтра областей объекты, которые не соответствуют фильтру, будут пропущены во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="09823-109">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="09823-110">Фильтр является частью [сопоставления объектов](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="09823-110">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="09823-111">Он состоит из нескольких наборов групп фильтров, а каждая группа фильтра содержит одно или несколько предложений.</span><span class="sxs-lookup"><span data-stu-id="09823-111">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="09823-112">Объект рассматривается в области для группы (Группа оценивается как `true`) только в `true`том случае, если все предложения группы оцениваются.</span><span class="sxs-lookup"><span data-stu-id="09823-112">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="09823-113">Объект рассматривается в области для набора групп (набор групп оценивается как `true`), если для `true`каждой из групп в наборе вычислена значение.</span><span class="sxs-lookup"><span data-stu-id="09823-113">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="09823-114">Дополнительные сведения см в разделе [Подготовка приложений на основе атрибутов с помощью фильтров областей](/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="09823-114">For more information, see [Attribute-based application provisioning with scoping filters](/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="09823-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="09823-115">Properties</span></span>
| <span data-ttu-id="09823-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="09823-116">Property</span></span>     | <span data-ttu-id="09823-117">Тип</span><span class="sxs-lookup"><span data-stu-id="09823-117">Type</span></span>   |<span data-ttu-id="09823-118">Описание</span><span class="sxs-lookup"><span data-stu-id="09823-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09823-119">категорифилтерграупс</span><span class="sxs-lookup"><span data-stu-id="09823-119">categoryFilterGroups</span></span>|<span data-ttu-id="09823-120">Коллекция [филтерграуп](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="09823-120">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="09823-121">`*Experimental*`Набор групп фильтров, используемый, чтобы определить, принадлежит ли данный объект и должен ли он обрабатываться как часть этого сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="09823-121">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="09823-122">Объект считается в области действия, \*Если любая из групп в коллекции оценивается как `true` \*.</span><span class="sxs-lookup"><span data-stu-id="09823-122">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="09823-123">groups</span><span class="sxs-lookup"><span data-stu-id="09823-123">groups</span></span>|<span data-ttu-id="09823-124">Коллекция [филтерграуп](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="09823-124">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="09823-125">Набор групп фильтров, используемый для определения того, находится ли заданный объект в области для подготовки.</span><span class="sxs-lookup"><span data-stu-id="09823-125">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="09823-126">**Это фильтр, который следует использовать в большинстве случаев**.</span><span class="sxs-lookup"><span data-stu-id="09823-126">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="09823-127">Если объект, используемый для выполнения этого фильтра, в данный момент, а затем объект или фильтр изменились так, что фильтр не удовлетворен более длинным, такой объект \* будет передано.</span><span class="sxs-lookup"><span data-stu-id="09823-127">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="09823-128">Объект считается в области действия, \*Если любая из групп в коллекции оценивается как `true` \*.</span><span class="sxs-lookup"><span data-stu-id="09823-128">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="09823-129">инпутфилтерграупс</span><span class="sxs-lookup"><span data-stu-id="09823-129">inputFilterGroups</span></span>|<span data-ttu-id="09823-130">Коллекция [филтерграуп](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="09823-130">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="09823-131">`*Experimental*`Набор групп фильтров, используемый для фильтрации объектов на раннем этапе чтения их из каталога.</span><span class="sxs-lookup"><span data-stu-id="09823-131">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="09823-132">Если объект не соответствует этому фильтру, он не будет обрабатываться далее.</span><span class="sxs-lookup"><span data-stu-id="09823-132">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="09823-133">Важно понимать, что если объект, используемый для выполнения этого фильтра, в данный момент, а затем объект или фильтр изменился, так как фильтр больше не удовлетворен, такой объект *не передается*.</span><span class="sxs-lookup"><span data-stu-id="09823-133">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="09823-134">Объект считается в области действия, \*Если любая из групп в коллекции оценивается как `true` \*.</span><span class="sxs-lookup"><span data-stu-id="09823-134">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09823-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09823-135">JSON representation</span></span>

<span data-ttu-id="09823-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09823-136">Here is a JSON representation of the resource.</span></span>

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
