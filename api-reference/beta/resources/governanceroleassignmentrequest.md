---
title: тип ресурса governanceRoleAssignmentRequest
description: Представляет запрос на операции назначения ролей в Privilegd Identity Management.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 889baa55f6f639537b278eff5ff4b93cbfc8a1f6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443099"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="8e0d4-103">тип ресурса governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e0d4-103">governanceRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="8e0d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e0d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e0d4-105">Представляет запрос на операции назначения ролей в Privilegd Identity Management.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="8e0d4-106">`governanceRoleAssignmentRequest` — это объект, моделируемый билетами, используемый для управления жизненным циклом назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-106">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="8e0d4-107">Он представляет намерения и решения пользователей и администраторов, а также обеспечивает гибкость, чтобы включить реализацию повторяющихся schduling, ворота утверждения и так далее, по сравнению с непосредственной разоблачения , и операций на `POST` `PUT` `DELETE` `governanceRoleAssignment` .</span><span class="sxs-lookup"><span data-stu-id="8e0d4-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="8e0d4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8e0d4-108">Methods</span></span>

| <span data-ttu-id="8e0d4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8e0d4-109">Method</span></span>          |<span data-ttu-id="8e0d4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e0d4-110">Return Type</span></span>  |<span data-ttu-id="8e0d4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e0d4-111">Description</span></span>|
|:------------|:--------|:--------|
|<span data-ttu-id="8e0d4-112">[получение](../api/governanceroleassignmentrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="8e0d4-112">[Get](../api/governanceroleassignmentrequest-get.md)</span></span> | [<span data-ttu-id="8e0d4-113">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e0d4-113">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="8e0d4-114">Получите запрос на назначение ролей, указанный в ID.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-114">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="8e0d4-115">List</span><span class="sxs-lookup"><span data-stu-id="8e0d4-115">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="8e0d4-116">[коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8e0d4-116">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="8e0d4-117">Получить запросы на назначение ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-117">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="8e0d4-118">Создание</span><span class="sxs-lookup"><span data-stu-id="8e0d4-118">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="8e0d4-119">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e0d4-119">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="8e0d4-120">Создайте запрос для управления жизненным циклом существующего или нового назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-120">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="8e0d4-121">Отмена</span><span class="sxs-lookup"><span data-stu-id="8e0d4-121">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="8e0d4-122">Отмена ожидающих запросов на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-122">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="8e0d4-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="8e0d4-123">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="8e0d4-124">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e0d4-124">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="8e0d4-125">Администраторы обновляют решения по запросам, если запросы находятся в состоянии `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="8e0d4-125">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e0d4-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e0d4-126">Properties</span></span>
| <span data-ttu-id="8e0d4-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e0d4-127">Property</span></span>                  | <span data-ttu-id="8e0d4-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8e0d4-128">Type</span></span>          |<span data-ttu-id="8e0d4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8e0d4-129">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="8e0d4-130">id</span><span class="sxs-lookup"><span data-stu-id="8e0d4-130">id</span></span>                         |<span data-ttu-id="8e0d4-131">String</span><span class="sxs-lookup"><span data-stu-id="8e0d4-131">String</span></span>         |<span data-ttu-id="8e0d4-132">ID запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-132">The id of the role assignment request.</span></span>|
|<span data-ttu-id="8e0d4-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="8e0d4-133">resourceId</span></span>                 |<span data-ttu-id="8e0d4-134">String</span><span class="sxs-lookup"><span data-stu-id="8e0d4-134">String</span></span>         |<span data-ttu-id="8e0d4-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-135">Required.</span></span> <span data-ttu-id="8e0d4-136">ID ресурса, с которым связан запрос на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-136">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="8e0d4-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8e0d4-137">roleDefinitionId</span></span>           |<span data-ttu-id="8e0d4-138">String</span><span class="sxs-lookup"><span data-stu-id="8e0d4-138">String</span></span>         |<span data-ttu-id="8e0d4-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-139">Required.</span></span> <span data-ttu-id="8e0d4-140">Id определения роли, с которым связан запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-140">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="8e0d4-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="8e0d4-141">subjectId</span></span>                  |<span data-ttu-id="8e0d4-142">String</span><span class="sxs-lookup"><span data-stu-id="8e0d4-142">String</span></span>         |<span data-ttu-id="8e0d4-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-143">Required.</span></span> <span data-ttu-id="8e0d4-144">ID субъекта, с которым связан запрос на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-144">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="8e0d4-145">type</span><span class="sxs-lookup"><span data-stu-id="8e0d4-145">type</span></span>                       |<span data-ttu-id="8e0d4-146">String</span><span class="sxs-lookup"><span data-stu-id="8e0d4-146">String</span></span>         |<span data-ttu-id="8e0d4-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-147">Required.</span></span> <span data-ttu-id="8e0d4-148">Представление типа операции при назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-148">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="8e0d4-149">Значение может быть</span><span class="sxs-lookup"><span data-stu-id="8e0d4-149">The value can be</span></span> <ul><li><span data-ttu-id="8e0d4-150">`AdminAdd`: Администраторы назначают пользователям и группам роли;</span><span class="sxs-lookup"><span data-stu-id="8e0d4-150">`AdminAdd`: Administrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="8e0d4-151">`UserAdd`: Пользователи активируют подходящие назначения;</span><span class="sxs-lookup"><span data-stu-id="8e0d4-151">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="8e0d4-152">`AdminUpdate`: Администраторы изменяют существующие назначения ролей</span><span class="sxs-lookup"><span data-stu-id="8e0d4-152">`AdminUpdate`: Administrators change existing role assignments</span></span></li><li><span data-ttu-id="8e0d4-153">`AdminRemove`: Администраторы удаляют пользователей и группы из ролей;</span><span class="sxs-lookup"><span data-stu-id="8e0d4-153">`AdminRemove`: Administrators remove users/groups from roles;</span></span><li><span data-ttu-id="8e0d4-154">`UserRemove`: Пользователи деактивируют активные назначения;</span><span class="sxs-lookup"><span data-stu-id="8e0d4-154">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="8e0d4-155">`UserExtend`: Пользователи просят продлить срок действия назначений;</span><span class="sxs-lookup"><span data-stu-id="8e0d4-155">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="8e0d4-156">`AdminExtend`. Администраторы расширяют назначения по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-156">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="8e0d4-157">`UserRenew`: Пользователи просят продлить срок действия назначений;</span><span class="sxs-lookup"><span data-stu-id="8e0d4-157">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="8e0d4-158">`AdminRenew`. Администраторы расширяют назначения по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-158">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="8e0d4-159">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8e0d4-159">assignmentState</span></span>|<span data-ttu-id="8e0d4-160">String</span><span class="sxs-lookup"><span data-stu-id="8e0d4-160">String</span></span>  |<span data-ttu-id="8e0d4-161">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-161">Required.</span></span> <span data-ttu-id="8e0d4-162">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-162">The state of the assignment.</span></span> <span data-ttu-id="8e0d4-163">Значение может быть</span><span class="sxs-lookup"><span data-stu-id="8e0d4-163">The value can be</span></span> <ul><li> <span data-ttu-id="8e0d4-164">`Eligible` для назначения</span><span class="sxs-lookup"><span data-stu-id="8e0d4-164">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="8e0d4-165">`Active` - если оно непосредственно назначено администраторами или активировано при назначении, назначенное `Active` пользователями.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-165">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="8e0d4-166">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e0d4-166">requestedDateTime</span></span>          |<span data-ttu-id="8e0d4-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e0d4-167">DateTimeOffset</span></span> |<span data-ttu-id="8e0d4-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-168">Read-only.</span></span> <span data-ttu-id="8e0d4-169">Время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-169">The request create time.</span></span> <span data-ttu-id="8e0d4-170">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8e0d4-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8e0d4-171">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8e0d4-172">schedule</span><span class="sxs-lookup"><span data-stu-id="8e0d4-172">schedule</span></span>                   |[<span data-ttu-id="8e0d4-173">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8e0d4-173">governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="8e0d4-174">Объект расписания запроса назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-174">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="8e0d4-175">reason</span><span class="sxs-lookup"><span data-stu-id="8e0d4-175">reason</span></span>                     |<span data-ttu-id="8e0d4-176">String</span><span class="sxs-lookup"><span data-stu-id="8e0d4-176">String</span></span>         |<span data-ttu-id="8e0d4-177">Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-177">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="8e0d4-178">status</span><span class="sxs-lookup"><span data-stu-id="8e0d4-178">status</span></span>                     |[<span data-ttu-id="8e0d4-179">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="8e0d4-179">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="8e0d4-180">Состояние запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-180">The status of the role assignment request.</span></span>|
|<span data-ttu-id="8e0d4-181">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="8e0d4-181">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="8e0d4-182">String</span><span class="sxs-lookup"><span data-stu-id="8e0d4-182">String</span></span>        |<span data-ttu-id="8e0d4-183">Если это запрос на активацию роли, он представляет id `eligible assignment` переданного; В противном случае значение `null` .</span><span class="sxs-lookup"><span data-stu-id="8e0d4-183">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |



## <a name="relationships"></a><span data-ttu-id="8e0d4-184">Связи</span><span class="sxs-lookup"><span data-stu-id="8e0d4-184">Relationships</span></span>
| <span data-ttu-id="8e0d4-185">Связь</span><span class="sxs-lookup"><span data-stu-id="8e0d4-185">Relationship</span></span> | <span data-ttu-id="8e0d4-186">Тип</span><span class="sxs-lookup"><span data-stu-id="8e0d4-186">Type</span></span>                                |<span data-ttu-id="8e0d4-187">Описание</span><span class="sxs-lookup"><span data-stu-id="8e0d4-187">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="8e0d4-188">resource</span><span class="sxs-lookup"><span data-stu-id="8e0d4-188">resource</span></span>      |[<span data-ttu-id="8e0d4-189">governanceResource</span><span class="sxs-lookup"><span data-stu-id="8e0d4-189">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="8e0d4-190">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-190">Read-only.</span></span> <span data-ttu-id="8e0d4-191">Ресурс, на который направлен запрос.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-191">The resource that the request aims to.</span></span> |
|<span data-ttu-id="8e0d4-192">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e0d4-192">roleDefinition</span></span>|[<span data-ttu-id="8e0d4-193">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8e0d4-193">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="8e0d4-194">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-194">Read-only.</span></span> <span data-ttu-id="8e0d4-195">Определение роли, на которое направлен запрос.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-195">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="8e0d4-196">subject</span><span class="sxs-lookup"><span data-stu-id="8e0d4-196">subject</span></span>       |[<span data-ttu-id="8e0d4-197">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="8e0d4-197">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="8e0d4-198">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-198">Read-only.</span></span> <span data-ttu-id="8e0d4-199">Основной пользователь/группа.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-199">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="8e0d4-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e0d4-200">JSON representation</span></span>

<span data-ttu-id="8e0d4-201">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e0d4-201">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "type": "String",
  "assignmentState": "String",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


