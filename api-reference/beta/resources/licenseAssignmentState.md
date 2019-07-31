---
title: Тип ресурса Лиценсеассигнментстате
description: 'Свойство **лиценсеассигнментстатес** объекта user представляет собой коллекцию **лиценсеассигнментстате**. Он предоставляет пользователю сведения о назначении лицензий пользователю. Сведения включают в себя следующие сведения:  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d85b4e2d45739f0d82e11bf029d00cad91a0e726
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966957"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="31416-105">Тип ресурса Лиценсеассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31416-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31416-106">Свойство **лиценсеассигнментстатес** объекта [User](user.md) представляет собой коллекцию **лиценсеассигнментстате**.</span><span class="sxs-lookup"><span data-stu-id="31416-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="31416-107">Он предоставляет пользователю сведения о назначении лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="31416-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="31416-108">Сведения включают в себя следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="31416-108">The details includes information like:</span></span>  

- <span data-ttu-id="31416-109">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="31416-109">What plans are disabled for a user</span></span>
- <span data-ttu-id="31416-110">Указывает, была ли лицензия назначена пользователю напрямую или унаследована от группы.</span><span class="sxs-lookup"><span data-stu-id="31416-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="31416-111">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="31416-111">Current state of the assignment</span></span>
- <span data-ttu-id="31416-112">Если состояние назначения — Error (ошибка), каковы сведения об ошибке для сбоя?</span><span class="sxs-lookup"><span data-stu-id="31416-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="31416-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="31416-113">Properties</span></span>
| <span data-ttu-id="31416-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="31416-114">Property</span></span>     | <span data-ttu-id="31416-115">Тип</span><span class="sxs-lookup"><span data-stu-id="31416-115">Type</span></span>   |<span data-ttu-id="31416-116">Описание</span><span class="sxs-lookup"><span data-stu-id="31416-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31416-117">Ассигнедбиграуп</span><span class="sxs-lookup"><span data-stu-id="31416-117">assignedByGroup</span></span>|<span data-ttu-id="31416-118">string</span><span class="sxs-lookup"><span data-stu-id="31416-118">string</span></span>|<span data-ttu-id="31416-119">Идентификатор группы, которая назначает эту лицензию.</span><span class="sxs-lookup"><span data-stu-id="31416-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="31416-120">Если назначение относится к прямой назначенной лицензии, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="31416-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="31416-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31416-121">Read-Only.</span></span>|
|<span data-ttu-id="31416-122">Дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="31416-122">disabledPlans</span></span>|<span data-ttu-id="31416-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="31416-123">Collection(String)</span></span>|<span data-ttu-id="31416-124">Планы обслуживания, которые отключены в этом назначении.</span><span class="sxs-lookup"><span data-stu-id="31416-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="31416-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31416-125">Read-Only.</span></span>|
|<span data-ttu-id="31416-126">error</span><span class="sxs-lookup"><span data-stu-id="31416-126">error</span></span>|<span data-ttu-id="31416-127">String</span><span class="sxs-lookup"><span data-stu-id="31416-127">String</span></span>|<span data-ttu-id="31416-128">Ошибка при назначении лицензии.</span><span class="sxs-lookup"><span data-stu-id="31416-128">License assignment failure error.</span></span> <span data-ttu-id="31416-129">Если лицензия назначена успешно, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="31416-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="31416-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31416-130">Read-Only.</span></span> <span data-ttu-id="31416-131">Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation` `UniquenessViolation`, и `Others`.</span><span class="sxs-lookup"><span data-stu-id="31416-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="31416-132">Дополнительные сведения о том, как определять и устранять ошибки назначения лицензий, можно найти [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="31416-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="31416-133">skuId</span><span class="sxs-lookup"><span data-stu-id="31416-133">skuId</span></span>|<span data-ttu-id="31416-134">String</span><span class="sxs-lookup"><span data-stu-id="31416-134">String</span></span>|<span data-ttu-id="31416-135">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="31416-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="31416-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31416-136">Read-Only.</span></span>|
|<span data-ttu-id="31416-137">state</span><span class="sxs-lookup"><span data-stu-id="31416-137">state</span></span>|<span data-ttu-id="31416-138">String</span><span class="sxs-lookup"><span data-stu-id="31416-138">String</span></span>|<span data-ttu-id="31416-139">Указывает текущее состояние этого назначения.</span><span class="sxs-lookup"><span data-stu-id="31416-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="31416-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31416-140">Read-Only.</span></span> <span data-ttu-id="31416-141">Возможные значения: Active, Активевисеррор, Disabled и Error.</span><span class="sxs-lookup"><span data-stu-id="31416-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31416-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31416-142">JSON representation</span></span>

<span data-ttu-id="31416-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31416-143">Here is a JSON representation of the resource</span></span>

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
