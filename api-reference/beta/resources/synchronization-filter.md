---
title: Тип ресурса filter
description: Определяет объекты, которые необходимо подготовка к приложению.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8c461dffab9af810d20f6b866134ecc5d4238eb1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133933"
---
# <a name="filter-resource-type"></a><span data-ttu-id="66207-103">Тип ресурса filter</span><span class="sxs-lookup"><span data-stu-id="66207-103">filter resource type</span></span>

<span data-ttu-id="66207-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66207-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66207-105">Определяет объекты, которые необходимо подготовка к приложению.</span><span class="sxs-lookup"><span data-stu-id="66207-105">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="66207-106">Например, может потребоваться только подготовка пользователей, расположенных в США.</span><span class="sxs-lookup"><span data-stu-id="66207-106">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="66207-107">Если фильтр области присутствует, объекты, которые не удовлетворяют фильтру, будут пропускаться во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="66207-107">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="66207-108">Фильтр является частью [сопоставления объектов.](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="66207-108">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="66207-109">Она состоит из нескольких наборов групп фильтров, каждая из которых содержит одно или несколько предложений.</span><span class="sxs-lookup"><span data-stu-id="66207-109">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="66207-110">Объект рассматривается в области для группы (группа оценивается как ) только в том случае, если все предложения группы `true` оцениваются как `true` .</span><span class="sxs-lookup"><span data-stu-id="66207-110">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="66207-111">Объект считается в области для набора групп (групповая группа оценивается как ), если любая из групп в наборе `true` оценивается как `true` .</span><span class="sxs-lookup"><span data-stu-id="66207-111">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="66207-112">Дополнительные сведения см. в теме "Подготовка приложений на основе [атрибутов с помощью фильтров области"](/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="66207-112">For more information, see [Attribute-based application provisioning with scoping filters](/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="66207-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="66207-113">Properties</span></span>
| <span data-ttu-id="66207-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="66207-114">Property</span></span>     | <span data-ttu-id="66207-115">Тип</span><span class="sxs-lookup"><span data-stu-id="66207-115">Type</span></span>   |<span data-ttu-id="66207-116">Описание</span><span class="sxs-lookup"><span data-stu-id="66207-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66207-117">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="66207-117">categoryFilterGroups</span></span>|<span data-ttu-id="66207-118">[Коллекция filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="66207-118">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="66207-119">`*Experimental*` Набор групп фильтров, используемый для решения, принадлежит ли данный объект, и должен обрабатываться в рамках этого сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="66207-119">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="66207-120">Объект считается в *области, если любая из групп `true` в коллекции оценивается* как .</span><span class="sxs-lookup"><span data-stu-id="66207-120">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="66207-121">groups</span><span class="sxs-lookup"><span data-stu-id="66207-121">groups</span></span>|<span data-ttu-id="66207-122">[Коллекция filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="66207-122">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="66207-123">Набор групп фильтров, используемый для решения, находится ли заданный объект в области для предоставления.</span><span class="sxs-lookup"><span data-stu-id="66207-123">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="66207-124">**Это фильтр, который следует использовать в большинстве случаев.**</span><span class="sxs-lookup"><span data-stu-id="66207-124">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="66207-125">Если объект, используемый для удовлетворения этого фильтра в данный момент, а затем объект или фильтр был изменен таким образом, что фильтр больше не удовлетворяется, такой объект \*будет де-подготовка".</span><span class="sxs-lookup"><span data-stu-id="66207-125">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="66207-126">Объект считается в *области, если любая из групп `true` в коллекции оценивается* как .</span><span class="sxs-lookup"><span data-stu-id="66207-126">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="66207-127">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="66207-127">inputFilterGroups</span></span>|<span data-ttu-id="66207-128">[Коллекция filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="66207-128">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="66207-129">`*Experimental*` Набор групп фильтров, используемый для фильтрации объектов на ранней стадии чтения их из каталога.</span><span class="sxs-lookup"><span data-stu-id="66207-129">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="66207-130">Если объект не удовлетворяет этому фильтру, он не будет обрабатываться далее.</span><span class="sxs-lookup"><span data-stu-id="66207-130">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="66207-131">Важно понимать, что если объект, используемый для удовлетворения этого фильтра в данный момент, а затем объект или фильтр был изменен таким образом, чтобы фильтр больше не удовлетворялся, такой объект *НЕ* будет отдан.</span><span class="sxs-lookup"><span data-stu-id="66207-131">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="66207-132">Объект считается в *области, если любая из групп `true` в коллекции оценивается* как .</span><span class="sxs-lookup"><span data-stu-id="66207-132">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66207-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="66207-133">JSON representation</span></span>

<span data-ttu-id="66207-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66207-134">Here is a JSON representation of the resource.</span></span>

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


