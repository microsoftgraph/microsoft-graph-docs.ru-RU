---
title: licenseAssignmentState type
description: 'Свойство **licenseAssignmentStates** объекта пользователя — это коллекция **лицензийAssignmentState.** Он предоставляет сведения о назначениях лицензий пользователю. Подробные сведения включают следующие сведения:  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jpettere
ms.openlocfilehash: 6362737397d8f5b5c1643557bc7c834392b520ef
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720531"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="952a0-105">licenseAssignmentState type</span><span class="sxs-lookup"><span data-stu-id="952a0-105">licenseAssignmentState resource type</span></span>

<span data-ttu-id="952a0-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="952a0-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="952a0-107">Свойство **licenseAssignmentStates** объекта [](user.md) пользователя — это коллекция **лицензийAssignmentState.**</span><span class="sxs-lookup"><span data-stu-id="952a0-107">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="952a0-108">Он предоставляет сведения о назначениях лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="952a0-108">It provides details about license assignments to a user.</span></span> <span data-ttu-id="952a0-109">Подробные сведения включают следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="952a0-109">The details includes information like:</span></span>

- <span data-ttu-id="952a0-110">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="952a0-110">What plans are disabled for a user</span></span>
- <span data-ttu-id="952a0-111">Была ли лицензия назначена пользователю напрямую или унаследована от группы</span><span class="sxs-lookup"><span data-stu-id="952a0-111">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="952a0-112">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="952a0-112">Current state of the assignment</span></span>
- <span data-ttu-id="952a0-113">Если состояние назначения — ошибка, то какая деталь ошибки для сбоя?</span><span class="sxs-lookup"><span data-stu-id="952a0-113">If the assignment state is Error, what is the error detail for the failure?</span></span>


## <a name="properties"></a><span data-ttu-id="952a0-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="952a0-114">Properties</span></span>
| <span data-ttu-id="952a0-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="952a0-115">Property</span></span>     | <span data-ttu-id="952a0-116">Тип</span><span class="sxs-lookup"><span data-stu-id="952a0-116">Type</span></span>   |<span data-ttu-id="952a0-117">Описание</span><span class="sxs-lookup"><span data-stu-id="952a0-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="952a0-118">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="952a0-118">assignedByGroup</span></span>|<span data-ttu-id="952a0-119">Строка</span><span class="sxs-lookup"><span data-stu-id="952a0-119">string</span></span>|<span data-ttu-id="952a0-120">ID группы, которая назначает эту лицензию.</span><span class="sxs-lookup"><span data-stu-id="952a0-120">The id of the group that assigns this license.</span></span> <span data-ttu-id="952a0-121">Если назначение является прямо назначенной лицензией, это поле будет Null.</span><span class="sxs-lookup"><span data-stu-id="952a0-121">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="952a0-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="952a0-122">Read-Only.</span></span>|
|<span data-ttu-id="952a0-123">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="952a0-123">disabledPlans</span></span>|<span data-ttu-id="952a0-124">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="952a0-124">Collection(String)</span></span>|<span data-ttu-id="952a0-125">Планы служб, отключенные в этом назначении.</span><span class="sxs-lookup"><span data-stu-id="952a0-125">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="952a0-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="952a0-126">Read-Only.</span></span>|
|<span data-ttu-id="952a0-127">error</span><span class="sxs-lookup"><span data-stu-id="952a0-127">error</span></span>|<span data-ttu-id="952a0-128">String</span><span class="sxs-lookup"><span data-stu-id="952a0-128">String</span></span>|<span data-ttu-id="952a0-129">Ошибка сбоя назначения лицензии.</span><span class="sxs-lookup"><span data-stu-id="952a0-129">License assignment failure error.</span></span> <span data-ttu-id="952a0-130">Если лицензия назначена успешно, это поле будет Null.</span><span class="sxs-lookup"><span data-stu-id="952a0-130">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="952a0-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="952a0-131">Read-Only.</span></span> <span data-ttu-id="952a0-132">Возможные значения: `CountViolation` , , , , , и `MutuallyExclusiveViolation` `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` `Others` .</span><span class="sxs-lookup"><span data-stu-id="952a0-132">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="952a0-133">Дополнительные сведения о том, как выявлять и устранять ошибки назначения лицензий, см. [здесь.](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)</span><span class="sxs-lookup"><span data-stu-id="952a0-133">For more information on how to identify and resolve license assignment errors see [here](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="952a0-134">skuId</span><span class="sxs-lookup"><span data-stu-id="952a0-134">skuId</span></span>|<span data-ttu-id="952a0-135">String</span><span class="sxs-lookup"><span data-stu-id="952a0-135">String</span></span>|<span data-ttu-id="952a0-136">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="952a0-136">The unique identifier for the SKU.</span></span> <span data-ttu-id="952a0-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="952a0-137">Read-Only.</span></span>|
|<span data-ttu-id="952a0-138">state</span><span class="sxs-lookup"><span data-stu-id="952a0-138">state</span></span>|<span data-ttu-id="952a0-139">String</span><span class="sxs-lookup"><span data-stu-id="952a0-139">String</span></span>|<span data-ttu-id="952a0-140">Указать текущее состояние этого назначения.</span><span class="sxs-lookup"><span data-stu-id="952a0-140">Indicate the current state of this assignment.</span></span> <span data-ttu-id="952a0-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="952a0-141">Read-Only.</span></span> <span data-ttu-id="952a0-142">Возможные значения: Active, ActiveWithError, Disabled и Error.</span><span class="sxs-lookup"><span data-stu-id="952a0-142">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="952a0-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="952a0-143">JSON representation</span></span>

<span data-ttu-id="952a0-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="952a0-144">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": ["string"],
  "error": " String ",
  "skuId": "String ",
  "state": "String"
}

```