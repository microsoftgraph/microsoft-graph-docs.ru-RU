---
title: Тип ресурса Filter
description: Определяет, какие объекты должны быть подготовлены для приложения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c61ade97a2dd1da823fc48763040e0ee29573362
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029003"
---
# <a name="filter-resource-type"></a><span data-ttu-id="285bd-103">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="285bd-103">filter resource type</span></span>

<span data-ttu-id="285bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="285bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="285bd-105">Определяет, какие объекты должны быть подготовлены для приложения.</span><span class="sxs-lookup"><span data-stu-id="285bd-105">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="285bd-106">Например, вам может потребоваться предоставить только пользователей, которые находятся в США.</span><span class="sxs-lookup"><span data-stu-id="285bd-106">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="285bd-107">При наличии фильтра областей объекты, которые не соответствуют фильтру, будут пропущены во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="285bd-107">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="285bd-108">Фильтр является частью [сопоставления объектов](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="285bd-108">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="285bd-109">Он состоит из нескольких наборов групп фильтров, а каждая группа фильтра содержит одно или несколько предложений.</span><span class="sxs-lookup"><span data-stu-id="285bd-109">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="285bd-110">Объект рассматривается в области для группы (Группа оценивается как `true` ) только в том случае, если все предложения группы оцениваются `true` .</span><span class="sxs-lookup"><span data-stu-id="285bd-110">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="285bd-111">Объект рассматривается в области для набора групп (набор групп оценивается как `true` ), если для каждой из групп в наборе вычислена значение `true` .</span><span class="sxs-lookup"><span data-stu-id="285bd-111">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="285bd-112">Дополнительные сведения см в разделе [Подготовка приложений на основе атрибутов с помощью фильтров областей](/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="285bd-112">For more information, see [Attribute-based application provisioning with scoping filters](/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="285bd-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="285bd-113">Properties</span></span>
| <span data-ttu-id="285bd-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="285bd-114">Property</span></span>     | <span data-ttu-id="285bd-115">Тип</span><span class="sxs-lookup"><span data-stu-id="285bd-115">Type</span></span>   |<span data-ttu-id="285bd-116">Описание</span><span class="sxs-lookup"><span data-stu-id="285bd-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="285bd-117">категорифилтерграупс</span><span class="sxs-lookup"><span data-stu-id="285bd-117">categoryFilterGroups</span></span>|<span data-ttu-id="285bd-118">Коллекция [филтерграуп](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="285bd-118">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="285bd-119">`*Experimental*` Набор групп фильтров, используемый, чтобы определить, принадлежит ли данный объект и должен ли он обрабатываться как часть этого сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="285bd-119">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="285bd-120">Объект считается в области действия, \*Если любая из групп в коллекции оценивается как `true` \*.</span><span class="sxs-lookup"><span data-stu-id="285bd-120">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="285bd-121">groups</span><span class="sxs-lookup"><span data-stu-id="285bd-121">groups</span></span>|<span data-ttu-id="285bd-122">Коллекция [филтерграуп](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="285bd-122">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="285bd-123">Набор групп фильтров, используемый для определения того, находится ли заданный объект в области для подготовки.</span><span class="sxs-lookup"><span data-stu-id="285bd-123">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="285bd-124">**Это фильтр, который следует использовать в большинстве случаев**.</span><span class="sxs-lookup"><span data-stu-id="285bd-124">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="285bd-125">Если объект, используемый для выполнения этого фильтра, в данный момент, а затем объект или фильтр изменились так, что фильтр не удовлетворен более длинным, такой объект \* будет передано.</span><span class="sxs-lookup"><span data-stu-id="285bd-125">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="285bd-126">Объект считается в области действия, \*Если любая из групп в коллекции оценивается как `true` \*.</span><span class="sxs-lookup"><span data-stu-id="285bd-126">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="285bd-127">инпутфилтерграупс</span><span class="sxs-lookup"><span data-stu-id="285bd-127">inputFilterGroups</span></span>|<span data-ttu-id="285bd-128">Коллекция [филтерграуп](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="285bd-128">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="285bd-129">`*Experimental*` Набор групп фильтров, используемый для фильтрации объектов на раннем этапе чтения их из каталога.</span><span class="sxs-lookup"><span data-stu-id="285bd-129">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="285bd-130">Если объект не соответствует этому фильтру, он не будет обрабатываться далее.</span><span class="sxs-lookup"><span data-stu-id="285bd-130">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="285bd-131">Важно понимать, что если объект, используемый для выполнения этого фильтра, в данный момент, а затем объект или фильтр изменился, так как фильтр больше не удовлетворен, такой объект *не передается*.</span><span class="sxs-lookup"><span data-stu-id="285bd-131">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="285bd-132">Объект считается в области действия, \*Если любая из групп в коллекции оценивается как `true` \*.</span><span class="sxs-lookup"><span data-stu-id="285bd-132">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="285bd-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="285bd-133">JSON representation</span></span>

<span data-ttu-id="285bd-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="285bd-134">Here is a JSON representation of the resource.</span></span>

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


