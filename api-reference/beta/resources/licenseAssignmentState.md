---
title: Тип ресурса licenseAssignmentState
description: 'Свойство **licenseAssignmentStates** удостоверение пользователя — это коллекция **licenseAssignmentState**. Его предоставляет подробные сведения о назначениях лицензии для пользователя. Сведения о включает в себя сведения, например:  '
localization_priority: Normal
ms.openlocfilehash: 51ff878f356902362487eda36d17c1894c33e5f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855631"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="593ab-105">Тип ресурса licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="593ab-105">licenseAssignmentState resource type</span></span>

> <span data-ttu-id="593ab-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="593ab-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="593ab-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="593ab-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="593ab-108">Свойство **licenseAssignmentStates** удостоверение [пользователя](user.md) — это коллекция **licenseAssignmentState**.</span><span class="sxs-lookup"><span data-stu-id="593ab-108">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="593ab-109">Его предоставляет подробные сведения о назначениях лицензии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="593ab-109">It provides details about license assignments to a user.</span></span> <span data-ttu-id="593ab-110">Сведения о включает в себя сведения, например:</span><span class="sxs-lookup"><span data-stu-id="593ab-110">The details includes information like:</span></span>  

 - <span data-ttu-id="593ab-111">Какие планы отключены для пользователя</span><span class="sxs-lookup"><span data-stu-id="593ab-111">What plans are disabled for a user</span></span>
 - <span data-ttu-id="593ab-112">Ли назначенных пользователю напрямую или наследуется из группы лицензии</span><span class="sxs-lookup"><span data-stu-id="593ab-112">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="593ab-113">Текущее состояние назначения</span><span class="sxs-lookup"><span data-stu-id="593ab-113">Current state of the assignment</span></span>
 - <span data-ttu-id="593ab-114">Если состояние назначения ошибки, что такое описание ошибки для ошибки</span><span class="sxs-lookup"><span data-stu-id="593ab-114">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="593ab-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="593ab-115">Properties</span></span>
| <span data-ttu-id="593ab-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="593ab-116">Property</span></span>     | <span data-ttu-id="593ab-117">Тип</span><span class="sxs-lookup"><span data-stu-id="593ab-117">Type</span></span>   |<span data-ttu-id="593ab-118">Описание</span><span class="sxs-lookup"><span data-stu-id="593ab-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="593ab-119">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="593ab-119">assignedByGroup</span></span>|<span data-ttu-id="593ab-120">string</span><span class="sxs-lookup"><span data-stu-id="593ab-120">string</span></span>|<span data-ttu-id="593ab-121">Идентификатор группы, предназначенного для назначения данной лицензии.</span><span class="sxs-lookup"><span data-stu-id="593ab-121">The id of the group that assigns this license.</span></span> <span data-ttu-id="593ab-122">Если назначения лицензий назначенных прямым, это поле будет Null.</span><span class="sxs-lookup"><span data-stu-id="593ab-122">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="593ab-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="593ab-123">Read-Only.</span></span>|
|<span data-ttu-id="593ab-124">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="593ab-124">disabledPlans</span></span>|<span data-ttu-id="593ab-125">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="593ab-125">Collection(String)</span></span>|<span data-ttu-id="593ab-126">Планы обслуживания, которые отключены в этой назначения.</span><span class="sxs-lookup"><span data-stu-id="593ab-126">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="593ab-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="593ab-127">Read-Only.</span></span>|
|<span data-ttu-id="593ab-128">error</span><span class="sxs-lookup"><span data-stu-id="593ab-128">error</span></span>|<span data-ttu-id="593ab-129">Строка</span><span class="sxs-lookup"><span data-stu-id="593ab-129">String</span></span>|<span data-ttu-id="593ab-130">Сбой назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="593ab-130">License assignment failure error.</span></span> <span data-ttu-id="593ab-131">Если лицензия назначена успешно, в этом поле будет Null.</span><span class="sxs-lookup"><span data-stu-id="593ab-131">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="593ab-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="593ab-132">Read-Only.</span></span> <span data-ttu-id="593ab-133">Возможные значения: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, и `Others`.</span><span class="sxs-lookup"><span data-stu-id="593ab-133">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="593ab-134">Дополнительные сведения о том, как выявлять и исправлять назначение лицензий ошибки можно [здесь](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="593ab-134">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="593ab-135">skuId</span><span class="sxs-lookup"><span data-stu-id="593ab-135">skuId</span></span>|<span data-ttu-id="593ab-136">Строка</span><span class="sxs-lookup"><span data-stu-id="593ab-136">String</span></span>|<span data-ttu-id="593ab-137">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="593ab-137">The unique identifier for the SKU.</span></span> <span data-ttu-id="593ab-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="593ab-138">Read-Only.</span></span>|
|<span data-ttu-id="593ab-139">state</span><span class="sxs-lookup"><span data-stu-id="593ab-139">state</span></span>|<span data-ttu-id="593ab-140">Строка</span><span class="sxs-lookup"><span data-stu-id="593ab-140">String</span></span>|<span data-ttu-id="593ab-141">Указывает текущее состояние данного назначения.</span><span class="sxs-lookup"><span data-stu-id="593ab-141">Indicate the current state of this assignment.</span></span> <span data-ttu-id="593ab-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="593ab-142">Read-Only.</span></span> <span data-ttu-id="593ab-143">Возможные значения: активный, ActiveWithError, отключено и ошибки.</span><span class="sxs-lookup"><span data-stu-id="593ab-143">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="593ab-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="593ab-144">JSON representation</span></span>

<span data-ttu-id="593ab-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="593ab-145">Here is a JSON representation of the resource</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
