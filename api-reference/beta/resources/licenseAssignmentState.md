---
title: Тип ресурса licenseAssignmentState
description: 'Свойство **licenseAssignmentStates** удостоверение пользователя — это коллекция **licenseAssignmentState**. Его предоставляет подробные сведения о назначениях лицензии для пользователя. Сведения о включает в себя сведения, например:  '
localization_priority: Normal
ms.openlocfilehash: a33dce3550d5a842493b73c83e8222a579348c9a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515281"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="ff63f-105">Тип ресурса licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="ff63f-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff63f-106">Свойство **licenseAssignmentStates** удостоверение [пользователя](user.md) — это коллекция **licenseAssignmentState**.</span><span class="sxs-lookup"><span data-stu-id="ff63f-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="ff63f-107">Его предоставляет подробные сведения о назначениях лицензии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff63f-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="ff63f-108">Сведения о включает в себя сведения, например:</span><span class="sxs-lookup"><span data-stu-id="ff63f-108">The details includes information like:</span></span>  

 - <span data-ttu-id="ff63f-109">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="ff63f-109">What plans are disabled for a user</span></span>
 - <span data-ttu-id="ff63f-110">Ли назначенных пользователю напрямую или наследуется из группы лицензии</span><span class="sxs-lookup"><span data-stu-id="ff63f-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="ff63f-111">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="ff63f-111">Current state of the assignment</span></span>
 - <span data-ttu-id="ff63f-112">Если состояние назначения ошибки, что такое описание ошибки для ошибки</span><span class="sxs-lookup"><span data-stu-id="ff63f-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="ff63f-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff63f-113">Properties</span></span>
| <span data-ttu-id="ff63f-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff63f-114">Property</span></span>     | <span data-ttu-id="ff63f-115">Тип</span><span class="sxs-lookup"><span data-stu-id="ff63f-115">Type</span></span>   |<span data-ttu-id="ff63f-116">Описание</span><span class="sxs-lookup"><span data-stu-id="ff63f-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff63f-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="ff63f-117">assignedByGroup</span></span>|<span data-ttu-id="ff63f-118">string</span><span class="sxs-lookup"><span data-stu-id="ff63f-118">string</span></span>|<span data-ttu-id="ff63f-119">Идентификатор группы, предназначенного для назначения данной лицензии.</span><span class="sxs-lookup"><span data-stu-id="ff63f-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="ff63f-120">Если назначения лицензий назначенных прямым, это поле будет Null.</span><span class="sxs-lookup"><span data-stu-id="ff63f-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="ff63f-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff63f-121">Read-Only.</span></span>|
|<span data-ttu-id="ff63f-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="ff63f-122">disabledPlans</span></span>|<span data-ttu-id="ff63f-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="ff63f-123">Collection(String)</span></span>|<span data-ttu-id="ff63f-124">Планы обслуживания, которые отключены в этой назначения.</span><span class="sxs-lookup"><span data-stu-id="ff63f-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="ff63f-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff63f-125">Read-Only.</span></span>|
|<span data-ttu-id="ff63f-126">error</span><span class="sxs-lookup"><span data-stu-id="ff63f-126">error</span></span>|<span data-ttu-id="ff63f-127">String</span><span class="sxs-lookup"><span data-stu-id="ff63f-127">String</span></span>|<span data-ttu-id="ff63f-128">Сбой назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="ff63f-128">License assignment failure error.</span></span> <span data-ttu-id="ff63f-129">Если лицензия назначена успешно, в этом поле будет Null.</span><span class="sxs-lookup"><span data-stu-id="ff63f-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="ff63f-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff63f-130">Read-Only.</span></span> <span data-ttu-id="ff63f-131">Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, и `Others`.</span><span class="sxs-lookup"><span data-stu-id="ff63f-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="ff63f-132">Дополнительные сведения о том, как выявлять и исправлять назначение лицензий ошибки можно [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="ff63f-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="ff63f-133">skuId</span><span class="sxs-lookup"><span data-stu-id="ff63f-133">skuId</span></span>|<span data-ttu-id="ff63f-134">String</span><span class="sxs-lookup"><span data-stu-id="ff63f-134">String</span></span>|<span data-ttu-id="ff63f-135">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="ff63f-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="ff63f-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff63f-136">Read-Only.</span></span>|
|<span data-ttu-id="ff63f-137">state</span><span class="sxs-lookup"><span data-stu-id="ff63f-137">state</span></span>|<span data-ttu-id="ff63f-138">String</span><span class="sxs-lookup"><span data-stu-id="ff63f-138">String</span></span>|<span data-ttu-id="ff63f-139">Указывает текущее состояние данного назначения.</span><span class="sxs-lookup"><span data-stu-id="ff63f-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="ff63f-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff63f-140">Read-Only.</span></span> <span data-ttu-id="ff63f-141">Возможные значения: активный, ActiveWithError, отключено и ошибки.</span><span class="sxs-lookup"><span data-stu-id="ff63f-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff63f-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff63f-142">JSON representation</span></span>

<span data-ttu-id="ff63f-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff63f-143">Here is a JSON representation of the resource</span></span>

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
