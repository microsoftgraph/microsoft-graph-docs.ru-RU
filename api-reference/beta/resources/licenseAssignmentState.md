---
title: Тип ресурса Лиценсеассигнментстате
description: 'Свойство **лиценсеассигнментстатес** объекта user представляет собой коллекцию **лиценсеассигнментстате**. Он предоставляет пользователю сведения о назначении лицензий пользователю. Сведения включают в себя следующие сведения:  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: d20eaebd15a56b6a9f68c90265b039781b53ea20
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812816"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="3ed8f-105">Тип ресурса Лиценсеассигнментстате</span><span class="sxs-lookup"><span data-stu-id="3ed8f-105">licenseAssignmentState resource type</span></span>

<span data-ttu-id="3ed8f-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ed8f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ed8f-107">Свойство **лиценсеассигнментстатес** объекта [User](user.md) представляет собой коллекцию **лиценсеассигнментстате**.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-107">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="3ed8f-108">Он предоставляет пользователю сведения о назначении лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-108">It provides details about license assignments to a user.</span></span> <span data-ttu-id="3ed8f-109">Сведения включают в себя следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="3ed8f-109">The details includes information like:</span></span>

- <span data-ttu-id="3ed8f-110">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="3ed8f-110">What plans are disabled for a user</span></span>
- <span data-ttu-id="3ed8f-111">Указывает, была ли лицензия назначена пользователю напрямую или унаследована от группы.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-111">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="3ed8f-112">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="3ed8f-112">Current state of the assignment</span></span>
- <span data-ttu-id="3ed8f-113">Если состояние назначения — Error (ошибка), каковы сведения об ошибке для сбоя?</span><span class="sxs-lookup"><span data-stu-id="3ed8f-113">If the assignment state is Error, what is the error detail for the failure?</span></span>


## <a name="properties"></a><span data-ttu-id="3ed8f-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ed8f-114">Properties</span></span>
| <span data-ttu-id="3ed8f-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ed8f-115">Property</span></span>     | <span data-ttu-id="3ed8f-116">Тип</span><span class="sxs-lookup"><span data-stu-id="3ed8f-116">Type</span></span>   |<span data-ttu-id="3ed8f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3ed8f-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ed8f-118">ассигнедбиграуп</span><span class="sxs-lookup"><span data-stu-id="3ed8f-118">assignedByGroup</span></span>|<span data-ttu-id="3ed8f-119">string</span><span class="sxs-lookup"><span data-stu-id="3ed8f-119">string</span></span>|<span data-ttu-id="3ed8f-120">Идентификатор группы, которая назначает эту лицензию.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-120">The id of the group that assigns this license.</span></span> <span data-ttu-id="3ed8f-121">Если назначение относится к прямой назначенной лицензии, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-121">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="3ed8f-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-122">Read-Only.</span></span>|
|<span data-ttu-id="3ed8f-123">дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="3ed8f-123">disabledPlans</span></span>|<span data-ttu-id="3ed8f-124">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="3ed8f-124">Collection(String)</span></span>|<span data-ttu-id="3ed8f-125">Планы обслуживания, которые отключены в этом назначении.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-125">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="3ed8f-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-126">Read-Only.</span></span>|
|<span data-ttu-id="3ed8f-127">error</span><span class="sxs-lookup"><span data-stu-id="3ed8f-127">error</span></span>|<span data-ttu-id="3ed8f-128">String</span><span class="sxs-lookup"><span data-stu-id="3ed8f-128">String</span></span>|<span data-ttu-id="3ed8f-129">Ошибка при назначении лицензии.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-129">License assignment failure error.</span></span> <span data-ttu-id="3ed8f-130">Если лицензия назначена успешно, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-130">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="3ed8f-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-131">Read-Only.</span></span> <span data-ttu-id="3ed8f-132">Возможные значения: `CountViolation` , `MutuallyExclusiveViolation` , `DependencyViolation` , `ProhibitedInUsageLocationViolation` , `UniquenessViolation` и `Others` .</span><span class="sxs-lookup"><span data-stu-id="3ed8f-132">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="3ed8f-133">Дополнительные сведения о том, как определять и устранять ошибки назначения лицензий, можно найти [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="3ed8f-133">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="3ed8f-134">skuId</span><span class="sxs-lookup"><span data-stu-id="3ed8f-134">skuId</span></span>|<span data-ttu-id="3ed8f-135">String</span><span class="sxs-lookup"><span data-stu-id="3ed8f-135">String</span></span>|<span data-ttu-id="3ed8f-136">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-136">The unique identifier for the SKU.</span></span> <span data-ttu-id="3ed8f-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-137">Read-Only.</span></span>|
|<span data-ttu-id="3ed8f-138">state</span><span class="sxs-lookup"><span data-stu-id="3ed8f-138">state</span></span>|<span data-ttu-id="3ed8f-139">String</span><span class="sxs-lookup"><span data-stu-id="3ed8f-139">String</span></span>|<span data-ttu-id="3ed8f-140">Указывает текущее состояние этого назначения.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-140">Indicate the current state of this assignment.</span></span> <span data-ttu-id="3ed8f-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-141">Read-Only.</span></span> <span data-ttu-id="3ed8f-142">Возможные значения: Active, Активевисеррор, Disabled и Error.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-142">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ed8f-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3ed8f-143">JSON representation</span></span>

<span data-ttu-id="3ed8f-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ed8f-144">Here is a JSON representation of the resource</span></span>

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
