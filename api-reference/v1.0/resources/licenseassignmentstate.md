---
title: Тип ресурса licenseAssignmentState
description: Свойство **licenseAssignmentStates** удостоверение пользователя — это семейство объектов **licenseAssignmentState** . Его предоставляет подробные сведения о назначениях лицензии для пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649455"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="f64c0-104">Тип ресурса licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="f64c0-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="f64c0-105">Свойство **licenseAssignmentStates** удостоверение [пользователя](user.md) — это семейство объектов **licenseAssignmentState** .</span><span class="sxs-lookup"><span data-stu-id="f64c0-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="f64c0-106">Его предоставляет подробные сведения о назначениях лицензии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f64c0-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="f64c0-107">Эти сведения включают сведения о таких как:</span><span class="sxs-lookup"><span data-stu-id="f64c0-107">The details include information such as:</span></span>  

 - <span data-ttu-id="f64c0-108">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="f64c0-108">What plans are disabled for a user</span></span>
 - <span data-ttu-id="f64c0-109">Ли назначенных пользователю напрямую или наследуется из группы лицензии</span><span class="sxs-lookup"><span data-stu-id="f64c0-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="f64c0-110">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="f64c0-110">The current state of the assignment</span></span>
 - <span data-ttu-id="f64c0-111">Дополнительные сведения об ошибке, если состояние назначения — ошибка</span><span class="sxs-lookup"><span data-stu-id="f64c0-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="f64c0-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="f64c0-112">Properties</span></span>
| <span data-ttu-id="f64c0-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="f64c0-113">Property</span></span>     | <span data-ttu-id="f64c0-114">Тип</span><span class="sxs-lookup"><span data-stu-id="f64c0-114">Type</span></span>   |<span data-ttu-id="f64c0-115">Описание</span><span class="sxs-lookup"><span data-stu-id="f64c0-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f64c0-116">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="f64c0-116">assignedByGroup</span></span>|<span data-ttu-id="f64c0-117">string</span><span class="sxs-lookup"><span data-stu-id="f64c0-117">string</span></span>|<span data-ttu-id="f64c0-118">Идентификатор группы, предназначенного для назначения данной лицензии.</span><span class="sxs-lookup"><span data-stu-id="f64c0-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="f64c0-119">Если назначения лицензий назначенных прямым, это поле будет Null.</span><span class="sxs-lookup"><span data-stu-id="f64c0-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="f64c0-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f64c0-120">Read-Only.</span></span>|
|<span data-ttu-id="f64c0-121">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="f64c0-121">disabledPlans</span></span>|<span data-ttu-id="f64c0-122">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="f64c0-122">Collection(String)</span></span>|<span data-ttu-id="f64c0-123">Планы обслуживания, которые отключены в этой назначения.</span><span class="sxs-lookup"><span data-stu-id="f64c0-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="f64c0-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f64c0-124">Read-Only.</span></span>|
|<span data-ttu-id="f64c0-125">error</span><span class="sxs-lookup"><span data-stu-id="f64c0-125">error</span></span>|<span data-ttu-id="f64c0-126">String</span><span class="sxs-lookup"><span data-stu-id="f64c0-126">String</span></span>|<span data-ttu-id="f64c0-127">Сбой назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="f64c0-127">License assignment failure error.</span></span> <span data-ttu-id="f64c0-128">Если лицензия назначена успешно, в этом поле будет Null.</span><span class="sxs-lookup"><span data-stu-id="f64c0-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="f64c0-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f64c0-129">Read-Only.</span></span> <span data-ttu-id="f64c0-130">Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, и `Others`.</span><span class="sxs-lookup"><span data-stu-id="f64c0-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="f64c0-131">Дополнительные сведения о том, как выявлять и исправлять назначение лицензий ошибки можно [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="f64c0-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="f64c0-132">skuId</span><span class="sxs-lookup"><span data-stu-id="f64c0-132">skuId</span></span>|<span data-ttu-id="f64c0-133">String</span><span class="sxs-lookup"><span data-stu-id="f64c0-133">String</span></span>|<span data-ttu-id="f64c0-134">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="f64c0-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="f64c0-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f64c0-135">Read-Only.</span></span>|
|<span data-ttu-id="f64c0-136">state</span><span class="sxs-lookup"><span data-stu-id="f64c0-136">state</span></span>|<span data-ttu-id="f64c0-137">String</span><span class="sxs-lookup"><span data-stu-id="f64c0-137">String</span></span>|<span data-ttu-id="f64c0-138">Указывает текущее состояние данного назначения.</span><span class="sxs-lookup"><span data-stu-id="f64c0-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="f64c0-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f64c0-139">Read-Only.</span></span> <span data-ttu-id="f64c0-140">Возможные значения: активный, ActiveWithError, отключено и ошибки.</span><span class="sxs-lookup"><span data-stu-id="f64c0-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f64c0-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f64c0-141">JSON representation</span></span>

<span data-ttu-id="f64c0-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f64c0-142">The following is a JSON representation of the resource.</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
