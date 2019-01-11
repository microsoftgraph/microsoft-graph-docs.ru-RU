---
title: Тип ресурса фильтра
description: Определяет, какие объекты, следует подготовить к приложению. Например может потребоваться только подготовки пользователей, которые расположены в США. Если фильтр области видимости, объекты, которые не удовлетворяют фильтра будет пропущено во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 754271e9d33159a14d1abf356280dd619643002f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894413"
---
# <a name="filter-resource-type"></a><span data-ttu-id="521f6-105">Тип ресурса фильтра</span><span class="sxs-lookup"><span data-stu-id="521f6-105">filter resource type</span></span>

> <span data-ttu-id="521f6-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="521f6-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="521f6-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="521f6-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="521f6-108">Определяет, какие объекты, следует подготовить к приложению.</span><span class="sxs-lookup"><span data-stu-id="521f6-108">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="521f6-109">Например может потребоваться только подготовки пользователей, которые расположены в США.</span><span class="sxs-lookup"><span data-stu-id="521f6-109">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="521f6-110">Если фильтр области видимости, объекты, которые не удовлетворяют фильтра будет пропущено во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="521f6-110">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="521f6-111">Фильтр является частью [сопоставление объектов](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="521f6-111">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="521f6-112">Состоит из нескольких наборов групп фильтра, и каждой группе фильтра содержит одно или несколько предложений.</span><span class="sxs-lookup"><span data-stu-id="521f6-112">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="521f6-113">Объект считается в области действия группы (рассчитано группы для `true`) только в том случае, если все предложения группе вычисляются для `true`.</span><span class="sxs-lookup"><span data-stu-id="521f6-113">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="521f6-114">Объект считается в области действия для набора группы (набор групп вычисляется для `true`) Если какие-либо группы в наборе оценивается `true`.</span><span class="sxs-lookup"><span data-stu-id="521f6-114">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="521f6-115">Для получения дополнительных сведений см. [Подготовка с помощью области видимости фильтры приложения на основе атрибутов](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="521f6-115">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="521f6-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="521f6-116">Properties</span></span>
| <span data-ttu-id="521f6-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="521f6-117">Property</span></span>     | <span data-ttu-id="521f6-118">Тип</span><span class="sxs-lookup"><span data-stu-id="521f6-118">Type</span></span>   |<span data-ttu-id="521f6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="521f6-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="521f6-120">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="521f6-120">categoryFilterGroups</span></span>|<span data-ttu-id="521f6-121">[filterGroup](synchronization-filtergroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="521f6-121">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="521f6-122">`*Experimental*`Используются для определения, является ли указанный объект принадлежит группе установлен фильтр и будут обрабатываться как часть этого сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="521f6-122">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="521f6-123">Объект считается в области \*Если какие-либо группы в коллекции оценивается `true` \*.</span><span class="sxs-lookup"><span data-stu-id="521f6-123">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="521f6-124">группы</span><span class="sxs-lookup"><span data-stu-id="521f6-124">groups</span></span>|<span data-ttu-id="521f6-125">[filterGroup](synchronization-filtergroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="521f6-125">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="521f6-126">Фильтровать набор группы, используемый в том, является ли указанный объект в области действия для подготовки.</span><span class="sxs-lookup"><span data-stu-id="521f6-126">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="521f6-127">**Это фильтр, который должен использоваться в большинстве случаев**.</span><span class="sxs-lookup"><span data-stu-id="521f6-127">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="521f6-128">Объект, используемый для удовлетворения этот фильтр в данный момент и затем объект или фильтр был изменен, поэтому этот фильтр не больше, удовлетворены такого объекта \* будет получить отзыва подготовить к работе».</span><span class="sxs-lookup"><span data-stu-id="521f6-128">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="521f6-129">Объект считается в области \*Если какие-либо группы в коллекции оценивается `true` \*.</span><span class="sxs-lookup"><span data-stu-id="521f6-129">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="521f6-130">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="521f6-130">inputFilterGroups</span></span>|<span data-ttu-id="521f6-131">[filterGroup](synchronization-filtergroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="521f6-131">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="521f6-132">`*Experimental*`Фильтровать набор группы, используемый для фильтрации объектов на ранней стадии чтения их из каталога.</span><span class="sxs-lookup"><span data-stu-id="521f6-132">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="521f6-133">Если объект не удовлетворяют этот фильтр, которые не будут обрабатываться Дополнительно.</span><span class="sxs-lookup"><span data-stu-id="521f6-133">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="521f6-134">Важно понимать, что если объект используются для удовлетворения этот фильтр в данный момент, а затем объект или фильтр изменен, этот фильтр больше не выполняется, например объекта *будет не получите отзыва подготовить к работе*.</span><span class="sxs-lookup"><span data-stu-id="521f6-134">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="521f6-135">Объект считается в области \*Если какие-либо группы в коллекции оценивается `true` \*.</span><span class="sxs-lookup"><span data-stu-id="521f6-135">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="521f6-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="521f6-136">JSON representation</span></span>

<span data-ttu-id="521f6-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="521f6-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
