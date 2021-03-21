---
title: тип ресурса governanceRoleAssignmentRequest
description: Представляет запрос на операции назначения ролей в Priviledged Identity Management.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e96a0009c6108a77383fe770a6351d7b64efd6f7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961281"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="b4000-103">тип ресурса governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b4000-103">governanceRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="b4000-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4000-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4000-105">Представляет запрос на операции назначения ролей в Privilegd Identity Management.</span><span class="sxs-lookup"><span data-stu-id="b4000-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="b4000-106">`governanceRoleAssignmentRequest` — это объект, моделируемый билетами, используемый для управления жизненным циклом назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-106">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="b4000-107">Он представляет намерения и решения пользователей и администраторов, а также обеспечивает гибкость, чтобы включить реализацию повторяющихся schduling, ворота утверждения и так далее, по сравнению с непосредственной разоблачения , и операций на `POST` `PUT` `DELETE` `governanceRoleAssignment` .</span><span class="sxs-lookup"><span data-stu-id="b4000-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="b4000-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b4000-108">Methods</span></span>

| <span data-ttu-id="b4000-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b4000-109">Method</span></span>          |<span data-ttu-id="b4000-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b4000-110">Return Type</span></span>  |<span data-ttu-id="b4000-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b4000-111">Description</span></span>|
|:------------|:--------|:--------|
|<span data-ttu-id="b4000-112">[получение](../api/governanceroleassignmentrequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="b4000-112">[Get](../api/governanceroleassignmentrequest-get.md)</span></span> | [<span data-ttu-id="b4000-113">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b4000-113">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="b4000-114">Получите запрос на назначение ролей, указанный в ID.</span><span class="sxs-lookup"><span data-stu-id="b4000-114">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="b4000-115">List</span><span class="sxs-lookup"><span data-stu-id="b4000-115">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="b4000-116">[коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b4000-116">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="b4000-117">Получить запросы на назначение ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="b4000-117">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="b4000-118">Создание</span><span class="sxs-lookup"><span data-stu-id="b4000-118">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="b4000-119">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b4000-119">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="b4000-120">Создайте запрос для управления жизненным циклом существующего или нового назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-120">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="b4000-121">Отмена</span><span class="sxs-lookup"><span data-stu-id="b4000-121">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="b4000-122">Отмена ожидающих запросов на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-122">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="b4000-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="b4000-123">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="b4000-124">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b4000-124">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="b4000-125">Администраторы обновляют решения по запросам, если запросы находятся в состоянии `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="b4000-125">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="b4000-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4000-126">Properties</span></span>
| <span data-ttu-id="b4000-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4000-127">Property</span></span>                  | <span data-ttu-id="b4000-128">Тип</span><span class="sxs-lookup"><span data-stu-id="b4000-128">Type</span></span>          |<span data-ttu-id="b4000-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b4000-129">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="b4000-130">id</span><span class="sxs-lookup"><span data-stu-id="b4000-130">id</span></span>                         |<span data-ttu-id="b4000-131">Строка</span><span class="sxs-lookup"><span data-stu-id="b4000-131">String</span></span>         |<span data-ttu-id="b4000-132">ID запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-132">The id of the role assignment request.</span></span>|
|<span data-ttu-id="b4000-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="b4000-133">resourceId</span></span>                 |<span data-ttu-id="b4000-134">String</span><span class="sxs-lookup"><span data-stu-id="b4000-134">String</span></span>         |<span data-ttu-id="b4000-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4000-135">Required.</span></span> <span data-ttu-id="b4000-136">ID ресурса, с которым связан запрос на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-136">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="b4000-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b4000-137">roleDefinitionId</span></span>           |<span data-ttu-id="b4000-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b4000-138">String</span></span>         |<span data-ttu-id="b4000-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4000-139">Required.</span></span> <span data-ttu-id="b4000-140">Id определения роли, с которым связан запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-140">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="b4000-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="b4000-141">subjectId</span></span>                  |<span data-ttu-id="b4000-142">Строка</span><span class="sxs-lookup"><span data-stu-id="b4000-142">String</span></span>         |<span data-ttu-id="b4000-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4000-143">Required.</span></span> <span data-ttu-id="b4000-144">ID субъекта, с которым связан запрос на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-144">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="b4000-145">type</span><span class="sxs-lookup"><span data-stu-id="b4000-145">type</span></span>                       |<span data-ttu-id="b4000-146">String</span><span class="sxs-lookup"><span data-stu-id="b4000-146">String</span></span>        |<span data-ttu-id="b4000-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4000-147">Required.</span></span> <span data-ttu-id="b4000-148">Представление типа операции при назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-148">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="b4000-149">Возможные значения: `AdminAdd` `UserAdd` , , , , , , `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminExtend` `UserRenew` `AdminRenew` .</span><span class="sxs-lookup"><span data-stu-id="b4000-149">The possible values are: `AdminAdd` , `UserAdd` , `AdminUpdate` , `AdminRemove` , `UserRemove` , `UserExtend` , `AdminExtend` , `UserRenew` , `AdminRenew`.</span></span>|
|<span data-ttu-id="b4000-150">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b4000-150">assignmentState</span></span>|<span data-ttu-id="b4000-151">Строка</span><span class="sxs-lookup"><span data-stu-id="b4000-151">String</span></span>  |<span data-ttu-id="b4000-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4000-152">Required.</span></span> <span data-ttu-id="b4000-153">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="b4000-153">The state of the assignment.</span></span> <span data-ttu-id="b4000-154">Возможные значения: (для назначения, назначенного по назначению), (если оно непосредственно назначено) (администраторами или активировано при назначении, назначенное `Eligible`  `Active` `Active` пользователями).</span><span class="sxs-lookup"><span data-stu-id="b4000-154">The possible values are: `Eligible` (for eligible assignment),  `Active` (if it is directly assigned), `Active` (by administrators, or activated on an eligible assignment by the users).</span></span>|
|<span data-ttu-id="b4000-155">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4000-155">requestedDateTime</span></span>          |<span data-ttu-id="b4000-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4000-156">DateTimeOffset</span></span> |<span data-ttu-id="b4000-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4000-157">Read-only.</span></span> <span data-ttu-id="b4000-158">Время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="b4000-158">The request create time.</span></span> <span data-ttu-id="b4000-159">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b4000-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b4000-160">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b4000-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b4000-161">schedule</span><span class="sxs-lookup"><span data-stu-id="b4000-161">schedule</span></span>                   |[<span data-ttu-id="b4000-162">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b4000-162">governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="b4000-163">Объект расписания запроса назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-163">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="b4000-164">reason</span><span class="sxs-lookup"><span data-stu-id="b4000-164">reason</span></span>                     |<span data-ttu-id="b4000-165">Строка</span><span class="sxs-lookup"><span data-stu-id="b4000-165">String</span></span>         |<span data-ttu-id="b4000-166">Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости.</span><span class="sxs-lookup"><span data-stu-id="b4000-166">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="b4000-167">status</span><span class="sxs-lookup"><span data-stu-id="b4000-167">status</span></span>                     |[<span data-ttu-id="b4000-168">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="b4000-168">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="b4000-169">Состояние запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-169">The status of the role assignment request.</span></span>|
|<span data-ttu-id="b4000-170">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="b4000-170">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="b4000-171">Строка</span><span class="sxs-lookup"><span data-stu-id="b4000-171">String</span></span>        |<span data-ttu-id="b4000-172">Если это запрос на активацию роли, он представляет id `eligible assignment` переданного; В противном случае значение `null` .</span><span class="sxs-lookup"><span data-stu-id="b4000-172">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |

|<span data-ttu-id="b4000-173">Member</span><span class="sxs-lookup"><span data-stu-id="b4000-173">Member</span></span>|<span data-ttu-id="b4000-174">Описание</span><span class="sxs-lookup"><span data-stu-id="b4000-174">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b4000-175">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="b4000-175">AdminAdd</span></span>|<span data-ttu-id="b4000-176">Администраторы назначают пользователям/группам роли.</span><span class="sxs-lookup"><span data-stu-id="b4000-176">Administrators assign users/groups to roles.</span></span>|
|<span data-ttu-id="b4000-177">UserAdd</span><span class="sxs-lookup"><span data-stu-id="b4000-177">UserAdd</span></span>|<span data-ttu-id="b4000-178">Пользователи активируют подходящие назначения.</span><span class="sxs-lookup"><span data-stu-id="b4000-178">Users activate eligible assignments.</span></span>|
|<span data-ttu-id="b4000-179">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="b4000-179">AdminUpdate</span></span>|<span data-ttu-id="b4000-180">Администраторы изменяют существующие назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-180">Administrators change existing role assignments.</span></span>|
|<span data-ttu-id="b4000-181">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="b4000-181">AdminRemove</span></span>|<span data-ttu-id="b4000-182">Администраторы удаляют пользователей и группы из ролей.</span><span class="sxs-lookup"><span data-stu-id="b4000-182">Administrators remove users/groups from roles.</span></span>|
|<span data-ttu-id="b4000-183">UserRemove</span><span class="sxs-lookup"><span data-stu-id="b4000-183">UserRemove</span></span>|<span data-ttu-id="b4000-184">Пользователи отключат активные назначения.</span><span class="sxs-lookup"><span data-stu-id="b4000-184">Users deactivate active assignments.</span></span>|
|<span data-ttu-id="b4000-185">UserExtend</span><span class="sxs-lookup"><span data-stu-id="b4000-185">UserExtend</span></span>|<span data-ttu-id="b4000-186">Пользователи просят продлить срок действия назначений.</span><span class="sxs-lookup"><span data-stu-id="b4000-186">Users request to extend their expiring assignments.</span></span>|
|<span data-ttu-id="b4000-187">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="b4000-187">AdminExtend</span></span>|<span data-ttu-id="b4000-188">Администраторы расширяют назначения по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="b4000-188">Administrators extend expiring assignments.</span></span>|
|<span data-ttu-id="b4000-189">UserRenew</span><span class="sxs-lookup"><span data-stu-id="b4000-189">UserRenew</span></span>|<span data-ttu-id="b4000-190">Пользователи просят продлить истекаемы назначения.</span><span class="sxs-lookup"><span data-stu-id="b4000-190">Users request to renew their expired assignments.</span></span>|
|<span data-ttu-id="b4000-191">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="b4000-191">AdminRenew</span></span>|<span data-ttu-id="b4000-192">Администраторы расширяют назначения по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="b4000-192">Administrators extend expiring assignments.</span></span>|



## <a name="relationships"></a><span data-ttu-id="b4000-193">Связи</span><span class="sxs-lookup"><span data-stu-id="b4000-193">Relationships</span></span>
| <span data-ttu-id="b4000-194">Связь</span><span class="sxs-lookup"><span data-stu-id="b4000-194">Relationship</span></span> | <span data-ttu-id="b4000-195">Тип</span><span class="sxs-lookup"><span data-stu-id="b4000-195">Type</span></span>                                |<span data-ttu-id="b4000-196">Описание</span><span class="sxs-lookup"><span data-stu-id="b4000-196">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="b4000-197">resource</span><span class="sxs-lookup"><span data-stu-id="b4000-197">resource</span></span>      |[<span data-ttu-id="b4000-198">governanceResource</span><span class="sxs-lookup"><span data-stu-id="b4000-198">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="b4000-199">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4000-199">Read-only.</span></span> <span data-ttu-id="b4000-200">Ресурс, на который направлен запрос.</span><span class="sxs-lookup"><span data-stu-id="b4000-200">The resource that the request aims to.</span></span> |
|<span data-ttu-id="b4000-201">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b4000-201">roleDefinition</span></span>|[<span data-ttu-id="b4000-202">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b4000-202">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="b4000-203">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4000-203">Read-only.</span></span> <span data-ttu-id="b4000-204">Определение роли, на которое направлен запрос.</span><span class="sxs-lookup"><span data-stu-id="b4000-204">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="b4000-205">subject</span><span class="sxs-lookup"><span data-stu-id="b4000-205">subject</span></span>       |[<span data-ttu-id="b4000-206">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="b4000-206">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="b4000-207">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4000-207">Read-only.</span></span> <span data-ttu-id="b4000-208">Основной пользователь/группа.</span><span class="sxs-lookup"><span data-stu-id="b4000-208">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="b4000-209">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4000-209">JSON representation</span></span>

<span data-ttu-id="b4000-210">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4000-210">Here is a JSON representation of the resource.</span></span>

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


