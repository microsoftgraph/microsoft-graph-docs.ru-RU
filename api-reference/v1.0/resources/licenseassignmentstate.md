---
title: Тип ресурса Лиценсеассигнментстате
description: Свойство **лиценсеассигнментстатес** объекта User — коллекция объектов **лиценсеассигнментстате** . Он предоставляет пользователю сведения о назначении лицензий пользователю.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585148"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="a74a8-104">Тип ресурса Лиценсеассигнментстате</span><span class="sxs-lookup"><span data-stu-id="a74a8-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="a74a8-105">Свойство **лиценсеассигнментстатес** объекта [User](user.md) — коллекция объектов **лиценсеассигнментстате** .</span><span class="sxs-lookup"><span data-stu-id="a74a8-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="a74a8-106">Он предоставляет пользователю сведения о назначении лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="a74a8-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="a74a8-107">Сведения включают следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="a74a8-107">The details include information such as:</span></span>  

 - <span data-ttu-id="a74a8-108">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="a74a8-108">What plans are disabled for a user</span></span>
 - <span data-ttu-id="a74a8-109">Указывает, была ли лицензия назначена пользователю напрямую или унаследована от группы.</span><span class="sxs-lookup"><span data-stu-id="a74a8-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="a74a8-110">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="a74a8-110">The current state of the assignment</span></span>
 - <span data-ttu-id="a74a8-111">Сведения об ошибке, если состояние назначения — ошибка</span><span class="sxs-lookup"><span data-stu-id="a74a8-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="a74a8-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="a74a8-112">Properties</span></span>
| <span data-ttu-id="a74a8-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="a74a8-113">Property</span></span>     | <span data-ttu-id="a74a8-114">Тип</span><span class="sxs-lookup"><span data-stu-id="a74a8-114">Type</span></span>   |<span data-ttu-id="a74a8-115">Описание</span><span class="sxs-lookup"><span data-stu-id="a74a8-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a74a8-116">Ассигнедбиграуп</span><span class="sxs-lookup"><span data-stu-id="a74a8-116">assignedByGroup</span></span>|<span data-ttu-id="a74a8-117">строка</span><span class="sxs-lookup"><span data-stu-id="a74a8-117">string</span></span>|<span data-ttu-id="a74a8-118">Идентификатор группы, которая назначает эту лицензию.</span><span class="sxs-lookup"><span data-stu-id="a74a8-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="a74a8-119">Если назначение относится к прямой назначенной лицензии, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="a74a8-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="a74a8-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a74a8-120">Read-Only.</span></span>|
|<span data-ttu-id="a74a8-121">Дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="a74a8-121">disabledPlans</span></span>|<span data-ttu-id="a74a8-122">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="a74a8-122">Collection(String)</span></span>|<span data-ttu-id="a74a8-123">Планы обслуживания, которые отключены в этом назначении.</span><span class="sxs-lookup"><span data-stu-id="a74a8-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="a74a8-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a74a8-124">Read-Only.</span></span>|
|<span data-ttu-id="a74a8-125">error</span><span class="sxs-lookup"><span data-stu-id="a74a8-125">error</span></span>|<span data-ttu-id="a74a8-126">String</span><span class="sxs-lookup"><span data-stu-id="a74a8-126">String</span></span>|<span data-ttu-id="a74a8-127">Ошибка при назначении лицензии.</span><span class="sxs-lookup"><span data-stu-id="a74a8-127">License assignment failure error.</span></span> <span data-ttu-id="a74a8-128">Если лицензия назначена успешно, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="a74a8-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="a74a8-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a74a8-129">Read-Only.</span></span> <span data-ttu-id="a74a8-130">Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation` `UniquenessViolation`, и `Others`.</span><span class="sxs-lookup"><span data-stu-id="a74a8-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="a74a8-131">Дополнительные сведения о том, как определять и устранять ошибки назначения лицензий, можно найти [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="a74a8-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="a74a8-132">skuId</span><span class="sxs-lookup"><span data-stu-id="a74a8-132">skuId</span></span>|<span data-ttu-id="a74a8-133">String</span><span class="sxs-lookup"><span data-stu-id="a74a8-133">String</span></span>|<span data-ttu-id="a74a8-134">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="a74a8-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="a74a8-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a74a8-135">Read-Only.</span></span>|
|<span data-ttu-id="a74a8-136">state</span><span class="sxs-lookup"><span data-stu-id="a74a8-136">state</span></span>|<span data-ttu-id="a74a8-137">String</span><span class="sxs-lookup"><span data-stu-id="a74a8-137">String</span></span>|<span data-ttu-id="a74a8-138">Указывает текущее состояние этого назначения.</span><span class="sxs-lookup"><span data-stu-id="a74a8-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="a74a8-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a74a8-139">Read-Only.</span></span> <span data-ttu-id="a74a8-140">Возможные значения: Active, Активевисеррор, Disabled и Error.</span><span class="sxs-lookup"><span data-stu-id="a74a8-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a74a8-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a74a8-141">JSON representation</span></span>

<span data-ttu-id="a74a8-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a74a8-142">The following is a JSON representation of the resource.</span></span>

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
