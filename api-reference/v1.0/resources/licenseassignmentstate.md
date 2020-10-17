---
title: Тип ресурса Лиценсеассигнментстате
description: Свойство **лиценсеассигнментстатес** объекта User — коллекция объектов **лиценсеассигнментстате** . Он предоставляет пользователю сведения о назначении лицензий пользователю.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b26ab4be63cbb40929dbea3f40522ee4c6b7ff70
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582186"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="42c97-104">Тип ресурса Лиценсеассигнментстате</span><span class="sxs-lookup"><span data-stu-id="42c97-104">licenseAssignmentState resource type</span></span>

<span data-ttu-id="42c97-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42c97-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="42c97-106">Свойство **лиценсеассигнментстатес** объекта [User](user.md) — коллекция объектов **лиценсеассигнментстате** .</span><span class="sxs-lookup"><span data-stu-id="42c97-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="42c97-107">Он предоставляет пользователю сведения о назначении лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="42c97-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="42c97-108">Сведения включают следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="42c97-108">The details include information such as:</span></span>  

- <span data-ttu-id="42c97-109">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="42c97-109">What plans are disabled for a user</span></span>
- <span data-ttu-id="42c97-110">Указывает, была ли лицензия назначена пользователю напрямую или унаследована от группы.</span><span class="sxs-lookup"><span data-stu-id="42c97-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="42c97-111">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="42c97-111">The current state of the assignment</span></span>
- <span data-ttu-id="42c97-112">Сведения об ошибке, если состояние назначения — ошибка</span><span class="sxs-lookup"><span data-stu-id="42c97-112">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="42c97-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="42c97-113">Properties</span></span>
| <span data-ttu-id="42c97-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="42c97-114">Property</span></span>     | <span data-ttu-id="42c97-115">Тип</span><span class="sxs-lookup"><span data-stu-id="42c97-115">Type</span></span>   |<span data-ttu-id="42c97-116">Описание</span><span class="sxs-lookup"><span data-stu-id="42c97-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42c97-117">ассигнедбиграуп</span><span class="sxs-lookup"><span data-stu-id="42c97-117">assignedByGroup</span></span>|<span data-ttu-id="42c97-118">Строка</span><span class="sxs-lookup"><span data-stu-id="42c97-118">string</span></span>|<span data-ttu-id="42c97-119">Идентификатор группы, которая назначает эту лицензию.</span><span class="sxs-lookup"><span data-stu-id="42c97-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="42c97-120">Если назначение относится к прямой назначенной лицензии, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="42c97-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="42c97-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42c97-121">Read-Only.</span></span>|
|<span data-ttu-id="42c97-122">дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="42c97-122">disabledPlans</span></span>|<span data-ttu-id="42c97-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="42c97-123">Collection(String)</span></span>|<span data-ttu-id="42c97-124">Планы обслуживания, которые отключены в этом назначении.</span><span class="sxs-lookup"><span data-stu-id="42c97-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="42c97-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42c97-125">Read-Only.</span></span>|
|<span data-ttu-id="42c97-126">error</span><span class="sxs-lookup"><span data-stu-id="42c97-126">error</span></span>|<span data-ttu-id="42c97-127">String</span><span class="sxs-lookup"><span data-stu-id="42c97-127">String</span></span>|<span data-ttu-id="42c97-128">Ошибка при назначении лицензии.</span><span class="sxs-lookup"><span data-stu-id="42c97-128">License assignment failure error.</span></span> <span data-ttu-id="42c97-129">Если лицензия назначена успешно, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="42c97-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="42c97-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42c97-130">Read-Only.</span></span> <span data-ttu-id="42c97-131">Возможные значения: `CountViolation` , `MutuallyExclusiveViolation` , `DependencyViolation` , `ProhibitedInUsageLocationViolation` , `UniquenessViolation` и `Others` .</span><span class="sxs-lookup"><span data-stu-id="42c97-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="42c97-132">Дополнительные сведения о том, как определять и устранять ошибки назначения лицензий, можно найти [здесь](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="42c97-132">For more information on how to identify and resolve license assignment errors see [here](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="42c97-133">skuId</span><span class="sxs-lookup"><span data-stu-id="42c97-133">skuId</span></span>|<span data-ttu-id="42c97-134">String</span><span class="sxs-lookup"><span data-stu-id="42c97-134">String</span></span>|<span data-ttu-id="42c97-135">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="42c97-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="42c97-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42c97-136">Read-Only.</span></span>|
|<span data-ttu-id="42c97-137">state</span><span class="sxs-lookup"><span data-stu-id="42c97-137">state</span></span>|<span data-ttu-id="42c97-138">String</span><span class="sxs-lookup"><span data-stu-id="42c97-138">String</span></span>|<span data-ttu-id="42c97-139">Указывает текущее состояние этого назначения.</span><span class="sxs-lookup"><span data-stu-id="42c97-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="42c97-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42c97-140">Read-Only.</span></span> <span data-ttu-id="42c97-141">Возможные значения: Active, Активевисеррор, Disabled и Error.</span><span class="sxs-lookup"><span data-stu-id="42c97-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42c97-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42c97-142">JSON representation</span></span>

<span data-ttu-id="42c97-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42c97-143">The following is a JSON representation of the resource.</span></span>

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