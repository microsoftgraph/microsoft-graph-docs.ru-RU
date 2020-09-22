---
title: Тип ресурса Лиценсеассигнментстате
description: Свойство **лиценсеассигнментстатес** объекта User — коллекция объектов **лиценсеассигнментстате** . Он предоставляет пользователю сведения о назначении лицензий пользователю.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: c847528c9588d13cefb1c7ec0b29127c9175c9a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048325"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="7bde7-104">Тип ресурса Лиценсеассигнментстате</span><span class="sxs-lookup"><span data-stu-id="7bde7-104">licenseAssignmentState resource type</span></span>

<span data-ttu-id="7bde7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bde7-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="7bde7-106">Свойство **лиценсеассигнментстатес** объекта [User](user.md) — коллекция объектов **лиценсеассигнментстате** .</span><span class="sxs-lookup"><span data-stu-id="7bde7-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="7bde7-107">Он предоставляет пользователю сведения о назначении лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="7bde7-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="7bde7-108">Сведения включают следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="7bde7-108">The details include information such as:</span></span>  

- <span data-ttu-id="7bde7-109">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="7bde7-109">What plans are disabled for a user</span></span>
- <span data-ttu-id="7bde7-110">Указывает, была ли лицензия назначена пользователю напрямую или унаследована от группы.</span><span class="sxs-lookup"><span data-stu-id="7bde7-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="7bde7-111">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="7bde7-111">The current state of the assignment</span></span>
- <span data-ttu-id="7bde7-112">Сведения об ошибке, если состояние назначения — ошибка</span><span class="sxs-lookup"><span data-stu-id="7bde7-112">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="7bde7-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bde7-113">Properties</span></span>
| <span data-ttu-id="7bde7-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bde7-114">Property</span></span>     | <span data-ttu-id="7bde7-115">Тип</span><span class="sxs-lookup"><span data-stu-id="7bde7-115">Type</span></span>   |<span data-ttu-id="7bde7-116">Описание</span><span class="sxs-lookup"><span data-stu-id="7bde7-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bde7-117">ассигнедбиграуп</span><span class="sxs-lookup"><span data-stu-id="7bde7-117">assignedByGroup</span></span>|<span data-ttu-id="7bde7-118">string</span><span class="sxs-lookup"><span data-stu-id="7bde7-118">string</span></span>|<span data-ttu-id="7bde7-119">Идентификатор группы, которая назначает эту лицензию.</span><span class="sxs-lookup"><span data-stu-id="7bde7-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="7bde7-120">Если назначение относится к прямой назначенной лицензии, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="7bde7-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="7bde7-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bde7-121">Read-Only.</span></span>|
|<span data-ttu-id="7bde7-122">дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="7bde7-122">disabledPlans</span></span>|<span data-ttu-id="7bde7-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="7bde7-123">Collection(String)</span></span>|<span data-ttu-id="7bde7-124">Планы обслуживания, которые отключены в этом назначении.</span><span class="sxs-lookup"><span data-stu-id="7bde7-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="7bde7-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bde7-125">Read-Only.</span></span>|
|<span data-ttu-id="7bde7-126">error</span><span class="sxs-lookup"><span data-stu-id="7bde7-126">error</span></span>|<span data-ttu-id="7bde7-127">String</span><span class="sxs-lookup"><span data-stu-id="7bde7-127">String</span></span>|<span data-ttu-id="7bde7-128">Ошибка при назначении лицензии.</span><span class="sxs-lookup"><span data-stu-id="7bde7-128">License assignment failure error.</span></span> <span data-ttu-id="7bde7-129">Если лицензия назначена успешно, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="7bde7-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="7bde7-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bde7-130">Read-Only.</span></span> <span data-ttu-id="7bde7-131">Возможные значения: `CountViolation` , `MutuallyExclusiveViolation` , `DependencyViolation` , `ProhibitedInUsageLocationViolation` , `UniquenessViolation` и `Others` .</span><span class="sxs-lookup"><span data-stu-id="7bde7-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="7bde7-132">Дополнительные сведения о том, как определять и устранять ошибки назначения лицензий, можно найти [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="7bde7-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="7bde7-133">skuId</span><span class="sxs-lookup"><span data-stu-id="7bde7-133">skuId</span></span>|<span data-ttu-id="7bde7-134">String</span><span class="sxs-lookup"><span data-stu-id="7bde7-134">String</span></span>|<span data-ttu-id="7bde7-135">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="7bde7-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="7bde7-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bde7-136">Read-Only.</span></span>|
|<span data-ttu-id="7bde7-137">state</span><span class="sxs-lookup"><span data-stu-id="7bde7-137">state</span></span>|<span data-ttu-id="7bde7-138">String</span><span class="sxs-lookup"><span data-stu-id="7bde7-138">String</span></span>|<span data-ttu-id="7bde7-139">Указывает текущее состояние этого назначения.</span><span class="sxs-lookup"><span data-stu-id="7bde7-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="7bde7-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bde7-140">Read-Only.</span></span> <span data-ttu-id="7bde7-141">Возможные значения: Active, Активевисеррор, Disabled и Error.</span><span class="sxs-lookup"><span data-stu-id="7bde7-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bde7-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bde7-142">JSON representation</span></span>

<span data-ttu-id="7bde7-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bde7-143">The following is a JSON representation of the resource.</span></span>

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

