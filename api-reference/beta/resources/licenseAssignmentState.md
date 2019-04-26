---
title: Тип ресурса Лиценсеассигнментстате
description: 'Свойство **лиценсеассигнментстатес** объекта user представляет собой коллекцию **лиценсеассигнментстате**. Он предоставляет пользователю сведения о назначении лицензий пользователю. Сведения включают в себя следующие сведения:  '
localization_priority: Normal
ms.openlocfilehash: 1aa91dcb841c8f3219ba0ea00ad615777da89aa9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345361"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="31a81-105">Тип ресурса Лиценсеассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31a81-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31a81-106">Свойство **лиценсеассигнментстатес** объекта [User](user.md) представляет собой коллекцию **лиценсеассигнментстате**.</span><span class="sxs-lookup"><span data-stu-id="31a81-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="31a81-107">Он предоставляет пользователю сведения о назначении лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="31a81-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="31a81-108">Сведения включают в себя следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="31a81-108">The details includes information like:</span></span>  

 - <span data-ttu-id="31a81-109">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="31a81-109">What plans are disabled for a user</span></span>
 - <span data-ttu-id="31a81-110">Указывает, была ли лицензия назначена пользователю напрямую или унаследована от группы.</span><span class="sxs-lookup"><span data-stu-id="31a81-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="31a81-111">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="31a81-111">Current state of the assignment</span></span>
 - <span data-ttu-id="31a81-112">Если состояние назначения — Error (ошибка), каковы сведения об ошибке для сбоя?</span><span class="sxs-lookup"><span data-stu-id="31a81-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="31a81-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="31a81-113">Properties</span></span>
| <span data-ttu-id="31a81-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="31a81-114">Property</span></span>     | <span data-ttu-id="31a81-115">Тип</span><span class="sxs-lookup"><span data-stu-id="31a81-115">Type</span></span>   |<span data-ttu-id="31a81-116">Описание</span><span class="sxs-lookup"><span data-stu-id="31a81-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31a81-117">Ассигнедбиграуп</span><span class="sxs-lookup"><span data-stu-id="31a81-117">assignedByGroup</span></span>|<span data-ttu-id="31a81-118">строка</span><span class="sxs-lookup"><span data-stu-id="31a81-118">string</span></span>|<span data-ttu-id="31a81-119">Идентификатор группы, которая назначает эту лицензию.</span><span class="sxs-lookup"><span data-stu-id="31a81-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="31a81-120">Если назначение относится к прямой назначенной лицензии, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="31a81-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="31a81-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31a81-121">Read-Only.</span></span>|
|<span data-ttu-id="31a81-122">Дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="31a81-122">disabledPlans</span></span>|<span data-ttu-id="31a81-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="31a81-123">Collection(String)</span></span>|<span data-ttu-id="31a81-124">Планы обслуживания, которые отключены в этом назначении.</span><span class="sxs-lookup"><span data-stu-id="31a81-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="31a81-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31a81-125">Read-Only.</span></span>|
|<span data-ttu-id="31a81-126">error</span><span class="sxs-lookup"><span data-stu-id="31a81-126">error</span></span>|<span data-ttu-id="31a81-127">String</span><span class="sxs-lookup"><span data-stu-id="31a81-127">String</span></span>|<span data-ttu-id="31a81-128">Ошибка при назначении лицензии.</span><span class="sxs-lookup"><span data-stu-id="31a81-128">License assignment failure error.</span></span> <span data-ttu-id="31a81-129">Если лицензия назначена успешно, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="31a81-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="31a81-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31a81-130">Read-Only.</span></span> <span data-ttu-id="31a81-131">Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation` `UniquenessViolation`, и `Others`.</span><span class="sxs-lookup"><span data-stu-id="31a81-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="31a81-132">Дополнительные сведения о том, как определять и устранять ошибки назначения лицензий, можно найти [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="31a81-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="31a81-133">skuId</span><span class="sxs-lookup"><span data-stu-id="31a81-133">skuId</span></span>|<span data-ttu-id="31a81-134">String</span><span class="sxs-lookup"><span data-stu-id="31a81-134">String</span></span>|<span data-ttu-id="31a81-135">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="31a81-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="31a81-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31a81-136">Read-Only.</span></span>|
|<span data-ttu-id="31a81-137">state</span><span class="sxs-lookup"><span data-stu-id="31a81-137">state</span></span>|<span data-ttu-id="31a81-138">String</span><span class="sxs-lookup"><span data-stu-id="31a81-138">String</span></span>|<span data-ttu-id="31a81-139">Указывает текущее состояние этого назначения.</span><span class="sxs-lookup"><span data-stu-id="31a81-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="31a81-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31a81-140">Read-Only.</span></span> <span data-ttu-id="31a81-141">Возможные значения: Active, Активевисеррор, Disabled и Error.</span><span class="sxs-lookup"><span data-stu-id="31a81-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31a81-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="31a81-142">JSON representation</span></span>

<span data-ttu-id="31a81-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31a81-143">Here is a JSON representation of the resource</span></span>

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
