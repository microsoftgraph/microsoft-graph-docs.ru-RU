---
title: Тип ресурса Лиценсеассигнментстате
description: 'Свойство **лиценсеассигнментстатес** объекта user представляет собой коллекцию **лиценсеассигнментстате**. Он предоставляет пользователю сведения о назначении лицензий пользователю. Сведения включают в себя следующие сведения:  '
localization_priority: Normal
ms.openlocfilehash: e720070c4c97c58fd3c99e49656d7ca33f5fb9d4
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778434"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="cb5a1-105">Тип ресурса Лиценсеассигнментстате</span><span class="sxs-lookup"><span data-stu-id="cb5a1-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb5a1-106">Свойство **лиценсеассигнментстатес** объекта [User](user.md) представляет собой коллекцию **лиценсеассигнментстате**.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="cb5a1-107">Он предоставляет пользователю сведения о назначении лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="cb5a1-108">Сведения включают в себя следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="cb5a1-108">The details includes information like:</span></span>  

- <span data-ttu-id="cb5a1-109">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="cb5a1-109">What plans are disabled for a user</span></span>
- <span data-ttu-id="cb5a1-110">Указывает, была ли лицензия назначена пользователю напрямую или унаследована от группы.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="cb5a1-111">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="cb5a1-111">Current state of the assignment</span></span>
- <span data-ttu-id="cb5a1-112">Если состояние назначения — Error (ошибка), каковы сведения об ошибке для сбоя?</span><span class="sxs-lookup"><span data-stu-id="cb5a1-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="cb5a1-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb5a1-113">Properties</span></span>
| <span data-ttu-id="cb5a1-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb5a1-114">Property</span></span>     | <span data-ttu-id="cb5a1-115">Тип</span><span class="sxs-lookup"><span data-stu-id="cb5a1-115">Type</span></span>   |<span data-ttu-id="cb5a1-116">Описание</span><span class="sxs-lookup"><span data-stu-id="cb5a1-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb5a1-117">Ассигнедбиграуп</span><span class="sxs-lookup"><span data-stu-id="cb5a1-117">assignedByGroup</span></span>|<span data-ttu-id="cb5a1-118">string</span><span class="sxs-lookup"><span data-stu-id="cb5a1-118">string</span></span>|<span data-ttu-id="cb5a1-119">Идентификатор группы, которая назначает эту лицензию.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="cb5a1-120">Если назначение относится к прямой назначенной лицензии, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="cb5a1-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-121">Read-Only.</span></span>|
|<span data-ttu-id="cb5a1-122">Дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="cb5a1-122">disabledPlans</span></span>|<span data-ttu-id="cb5a1-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="cb5a1-123">Collection(String)</span></span>|<span data-ttu-id="cb5a1-124">Планы обслуживания, которые отключены в этом назначении.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="cb5a1-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-125">Read-Only.</span></span>|
|<span data-ttu-id="cb5a1-126">error</span><span class="sxs-lookup"><span data-stu-id="cb5a1-126">error</span></span>|<span data-ttu-id="cb5a1-127">String</span><span class="sxs-lookup"><span data-stu-id="cb5a1-127">String</span></span>|<span data-ttu-id="cb5a1-128">Ошибка при назначении лицензии.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-128">License assignment failure error.</span></span> <span data-ttu-id="cb5a1-129">Если лицензия назначена успешно, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="cb5a1-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-130">Read-Only.</span></span> <span data-ttu-id="cb5a1-131">Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation` `UniquenessViolation`, и `Others`.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="cb5a1-132">Дополнительные сведения о том, как определять и устранять ошибки назначения лицензий, можно найти [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="cb5a1-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="cb5a1-133">skuId</span><span class="sxs-lookup"><span data-stu-id="cb5a1-133">skuId</span></span>|<span data-ttu-id="cb5a1-134">String</span><span class="sxs-lookup"><span data-stu-id="cb5a1-134">String</span></span>|<span data-ttu-id="cb5a1-135">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="cb5a1-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-136">Read-Only.</span></span>|
|<span data-ttu-id="cb5a1-137">state</span><span class="sxs-lookup"><span data-stu-id="cb5a1-137">state</span></span>|<span data-ttu-id="cb5a1-138">String</span><span class="sxs-lookup"><span data-stu-id="cb5a1-138">String</span></span>|<span data-ttu-id="cb5a1-139">Указывает текущее состояние этого назначения.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="cb5a1-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-140">Read-Only.</span></span> <span data-ttu-id="cb5a1-141">Возможные значения: Active, Активевисеррор, Disabled и Error.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb5a1-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb5a1-142">JSON representation</span></span>

<span data-ttu-id="cb5a1-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb5a1-143">Here is a JSON representation of the resource</span></span>

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
