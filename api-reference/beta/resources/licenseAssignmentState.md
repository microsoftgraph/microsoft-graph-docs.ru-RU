---
title: Тип ресурса Лиценсеассигнментстате
description: 'Свойство **лиценсеассигнментстатес** объекта user представляет собой коллекцию **лиценсеассигнментстате**. Он предоставляет пользователю сведения о назначении лицензий пользователю. Сведения включают в себя следующие сведения:  '
localization_priority: Normal
ms.openlocfilehash: a33dce3550d5a842493b73c83e8222a579348c9a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581109"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="2e543-105">Тип ресурса Лиценсеассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2e543-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e543-106">Свойство **лиценсеассигнментстатес** объекта [User](user.md) представляет собой коллекцию **лиценсеассигнментстате**.</span><span class="sxs-lookup"><span data-stu-id="2e543-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="2e543-107">Он предоставляет пользователю сведения о назначении лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="2e543-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="2e543-108">Сведения включают в себя следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="2e543-108">The details includes information like:</span></span>  

 - <span data-ttu-id="2e543-109">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="2e543-109">What plans are disabled for a user</span></span>
 - <span data-ttu-id="2e543-110">Указывает, была ли лицензия назначена пользователю напрямую или унаследована от группы.</span><span class="sxs-lookup"><span data-stu-id="2e543-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="2e543-111">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="2e543-111">Current state of the assignment</span></span>
 - <span data-ttu-id="2e543-112">Если состояние назначения — Error (ошибка), каковы сведения об ошибке для сбоя?</span><span class="sxs-lookup"><span data-stu-id="2e543-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="2e543-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e543-113">Properties</span></span>
| <span data-ttu-id="2e543-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e543-114">Property</span></span>     | <span data-ttu-id="2e543-115">Тип</span><span class="sxs-lookup"><span data-stu-id="2e543-115">Type</span></span>   |<span data-ttu-id="2e543-116">Описание</span><span class="sxs-lookup"><span data-stu-id="2e543-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e543-117">Ассигнедбиграуп</span><span class="sxs-lookup"><span data-stu-id="2e543-117">assignedByGroup</span></span>|<span data-ttu-id="2e543-118">string</span><span class="sxs-lookup"><span data-stu-id="2e543-118">string</span></span>|<span data-ttu-id="2e543-119">Идентификатор группы, которая назначает эту лицензию.</span><span class="sxs-lookup"><span data-stu-id="2e543-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="2e543-120">Если назначение относится к прямой назначенной лицензии, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="2e543-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="2e543-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e543-121">Read-Only.</span></span>|
|<span data-ttu-id="2e543-122">Дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="2e543-122">disabledPlans</span></span>|<span data-ttu-id="2e543-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="2e543-123">Collection(String)</span></span>|<span data-ttu-id="2e543-124">Планы обслуживания, которые отключены в этом назначении.</span><span class="sxs-lookup"><span data-stu-id="2e543-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="2e543-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e543-125">Read-Only.</span></span>|
|<span data-ttu-id="2e543-126">error</span><span class="sxs-lookup"><span data-stu-id="2e543-126">error</span></span>|<span data-ttu-id="2e543-127">String</span><span class="sxs-lookup"><span data-stu-id="2e543-127">String</span></span>|<span data-ttu-id="2e543-128">Ошибка при назначении лицензии.</span><span class="sxs-lookup"><span data-stu-id="2e543-128">License assignment failure error.</span></span> <span data-ttu-id="2e543-129">Если лицензия назначена успешно, это поле будет иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="2e543-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="2e543-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e543-130">Read-Only.</span></span> <span data-ttu-id="2e543-131">Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation` `UniquenessViolation`, и `Others`.</span><span class="sxs-lookup"><span data-stu-id="2e543-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="2e543-132">Дополнительные сведения о том, как определять и устранять ошибки назначения лицензий, можно найти [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="2e543-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="2e543-133">skuId</span><span class="sxs-lookup"><span data-stu-id="2e543-133">skuId</span></span>|<span data-ttu-id="2e543-134">String</span><span class="sxs-lookup"><span data-stu-id="2e543-134">String</span></span>|<span data-ttu-id="2e543-135">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="2e543-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="2e543-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e543-136">Read-Only.</span></span>|
|<span data-ttu-id="2e543-137">state</span><span class="sxs-lookup"><span data-stu-id="2e543-137">state</span></span>|<span data-ttu-id="2e543-138">String</span><span class="sxs-lookup"><span data-stu-id="2e543-138">String</span></span>|<span data-ttu-id="2e543-139">Указывает текущее состояние этого назначения.</span><span class="sxs-lookup"><span data-stu-id="2e543-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="2e543-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e543-140">Read-Only.</span></span> <span data-ttu-id="2e543-141">Возможные значения: Active, Активевисеррор, Disabled и Error.</span><span class="sxs-lookup"><span data-stu-id="2e543-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e543-142">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2e543-142">JSON representation</span></span>

<span data-ttu-id="2e543-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e543-143">Here is a JSON representation of the resource</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
