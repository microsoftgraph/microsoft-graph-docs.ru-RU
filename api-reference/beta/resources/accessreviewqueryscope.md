---
title: тип ресурса accessReviewQueryScope
description: Определяет, что будет рассмотрено в обзоре доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 976a856755b6bb638719bec6006c3d8d0587c42a
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469798"
---
# <a name="accessreviewqueryscope-resource-type"></a><span data-ttu-id="8f687-103">тип ресурса accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="8f687-103">accessReviewQueryScope resource type</span></span>

<span data-ttu-id="8f687-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f687-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="8f687-105">Объект accessReviewQueryScope определяет, что будет рассмотрено в [accessReview.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="8f687-105">An accessReviewQueryScope object defines what will be reviewed in an [accessReview](../resources/accessreviewsv2-root.md).</span></span> <span data-ttu-id="8f687-106">В поддерживаемых запросах см. параметры выбора.</span><span class="sxs-lookup"><span data-stu-id="8f687-106">See the supported queries to see the selection options.</span></span> <span data-ttu-id="8f687-107">Чтобы просмотреть обзор доступа для неактивных пользователей, см. [в примере accessReviewInactiveUserQueryScope.](../resources/accessreviewinactiveusersqueryscope.md)</span><span class="sxs-lookup"><span data-stu-id="8f687-107">To scope an access review to inactive users, see [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span> 

<span data-ttu-id="8f687-108">Наследует [от accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="8f687-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8f687-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f687-109">Properties</span></span>
|<span data-ttu-id="8f687-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f687-110">Property</span></span>|<span data-ttu-id="8f687-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8f687-111">Type</span></span>|<span data-ttu-id="8f687-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8f687-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f687-113">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f687-113">query</span></span>|<span data-ttu-id="8f687-114">String</span><span class="sxs-lookup"><span data-stu-id="8f687-114">String</span></span>|<span data-ttu-id="8f687-115">Запрос, представляющий то, что будет рассмотрено в обзоре доступа.</span><span class="sxs-lookup"><span data-stu-id="8f687-115">The query representing what will be reviewed in an access review.</span></span> <span data-ttu-id="8f687-116">Примеры этого включают /groups/{id}/members?$filter=...</span><span class="sxs-lookup"><span data-stu-id="8f687-116">Examples of this include /groups/{id}/members?$filter=…</span></span>|
|<span data-ttu-id="8f687-117">queryRoot</span><span class="sxs-lookup"><span data-stu-id="8f687-117">queryRoot</span></span>|<span data-ttu-id="8f687-118">String</span><span class="sxs-lookup"><span data-stu-id="8f687-118">String</span></span>|<span data-ttu-id="8f687-119">В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса.</span><span class="sxs-lookup"><span data-stu-id="8f687-119">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="8f687-120">Это свойство необходимо только в том случае, если указан относительный запрос.</span><span class="sxs-lookup"><span data-stu-id="8f687-120">This property is only required if a relative query is specified.</span></span> <span data-ttu-id="8f687-121">Например, `./manager`.</span><span class="sxs-lookup"><span data-stu-id="8f687-121">For example, `./manager`.</span></span>|
|<span data-ttu-id="8f687-122">queryType</span><span class="sxs-lookup"><span data-stu-id="8f687-122">queryType</span></span>|<span data-ttu-id="8f687-123">String</span><span class="sxs-lookup"><span data-stu-id="8f687-123">String</span></span>|<span data-ttu-id="8f687-124">Указывает тип запроса.</span><span class="sxs-lookup"><span data-stu-id="8f687-124">Indicates the type of query.</span></span> <span data-ttu-id="8f687-125">Типы включают MicrosoftGraph и ARM.</span><span class="sxs-lookup"><span data-stu-id="8f687-125">Types include MicrosoftGraph and ARM.</span></span>|

### <a name="supported-queries-for-accessreviewqueryscope-as-scope"></a><span data-ttu-id="8f687-126">Поддерживаемые запросы для accessReviewQueryScope в качестве области</span><span class="sxs-lookup"><span data-stu-id="8f687-126">Supported queries for accessReviewQueryScope as scope</span></span>
<span data-ttu-id="8f687-127">Запросы поддерживаются как `scope` свойство [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8f687-127">The queries are supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="8f687-128">Сценарий</span><span class="sxs-lookup"><span data-stu-id="8f687-128">Scenario</span></span>| <span data-ttu-id="8f687-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f687-129">Query</span></span> | <span data-ttu-id="8f687-130">Дополнительные комментарии</span><span class="sxs-lookup"><span data-stu-id="8f687-130">Additional Comments</span></span> |
|--|--|-- |
| <span data-ttu-id="8f687-131">Просмотр всех пользователей, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="8f687-131">Review of all users assigned to a group</span></span> | <span data-ttu-id="8f687-132">/groups/{group id}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="8f687-132">/groups/{group id}/transitiveMembers</span></span> ||
| <span data-ttu-id="8f687-133">Просмотр гостевых пользователей, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="8f687-133">Review of guest users assigned to a group</span></span> | <span data-ttu-id="8f687-134">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="8f687-134">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> ||
| <span data-ttu-id="8f687-135">Обзор гостевых пользователей, присвоенных всем группам Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8f687-135">Review of guest users assigned to all Microsoft 365 groups</span></span> | <span data-ttu-id="8f687-136">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="8f687-136">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> | <span data-ttu-id="8f687-137">Обратите внимание, что соответствующий экземплярEnumerationScope также следует передать в accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8f687-137">Note that the corresponding instanceEnumerationScope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="8f687-138">См. таблицу ниже, например запросEnumerationScope.</span><span class="sxs-lookup"><span data-stu-id="8f687-138">See table below for instanceEnumerationScope query.</span></span> |
| <span data-ttu-id="8f687-139">Отзывы о назначении пакета назначения пакета управления правами</span><span class="sxs-lookup"><span data-stu-id="8f687-139">Entitlement Management Access Package Assignment Reviews</span></span> | <span data-ttu-id="8f687-140">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span><span class="sxs-lookup"><span data-stu-id="8f687-140">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span></span>| <span data-ttu-id="8f687-141">Обратите внимание, что только READ поддерживается для отзывов о назначении пакета доступа</span><span class="sxs-lookup"><span data-stu-id="8f687-141">Note that only READ is supported for Access Package Assignment Reviews</span></span>|
| <span data-ttu-id="8f687-142">Обзор директоров служб, назначенных привилегированным ролям</span><span class="sxs-lookup"><span data-stu-id="8f687-142">Review of Service Principals assigned to privileged roles</span></span> | <span data-ttu-id="8f687-143">/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')</span><span class="sxs-lookup"><span data-stu-id="8f687-143">/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')</span></span> | |

### <a name="supported-queries-for-instanceenumerationscope"></a><span data-ttu-id="8f687-144">Поддерживаемые запросы, напримерEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="8f687-144">Supported queries for instanceEnumerationScope</span></span> 
<span data-ttu-id="8f687-145">Запросы поддерживаются как `instanceEnumerationScope` свойство [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8f687-145">The queries are supported as the `instanceEnumerationScope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="8f687-146">Сценарий</span><span class="sxs-lookup"><span data-stu-id="8f687-146">Scenario</span></span>| <span data-ttu-id="8f687-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f687-147">Query</span></span> | <span data-ttu-id="8f687-148">Дополнительные комментарии</span><span class="sxs-lookup"><span data-stu-id="8f687-148">Additional Comments</span></span> |
|--|--|--|
|  <span data-ttu-id="8f687-149">Обзор гостевых пользователей, присвоенных всем группам Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8f687-149">Review of guest users assigned to all Microsoft 365 groups</span></span>| <span data-ttu-id="8f687-150">/v1.0/groups? \$ filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true</span><span class="sxs-lookup"><span data-stu-id="8f687-150">/v1.0/groups?\$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true</span></span> | <span data-ttu-id="8f687-151">Обратите внимание, что соответствующая область также должна быть передана вместе с этим</span><span class="sxs-lookup"><span data-stu-id="8f687-151">Note that the corresponding scope should also be passed in along with this</span></span>|
| <span data-ttu-id="8f687-152">Просмотр гостевых пользователей, назначенных всем группам</span><span class="sxs-lookup"><span data-stu-id="8f687-152">Review of guest users assigned to all teams</span></span> | <span data-ttu-id="8f687-153">/v1.0/groups? \$ filter=(groupTypes/any(c:c+eq+'Unified) и resourceProvisioningOptions/Any (x:x eq 'Team'))&$count=true</span><span class="sxs-lookup"><span data-stu-id="8f687-153">/v1.0/groups?\$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team'))&$count=true</span></span> | <span data-ttu-id="8f687-154">Обратите внимание, что соответствующая область также должна быть передана вместе с этим</span><span class="sxs-lookup"><span data-stu-id="8f687-154">Note that the corresponding scope should also be passed in along with this</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f687-155">Связи</span><span class="sxs-lookup"><span data-stu-id="8f687-155">Relationships</span></span>
<span data-ttu-id="8f687-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8f687-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f687-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8f687-157">JSON representation</span></span>
<span data-ttu-id="8f687-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f687-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
