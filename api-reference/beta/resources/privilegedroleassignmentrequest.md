---
title: тип ресурса privilegedRoleAssignmentRequest
description: Представляет запрос на операции назначения ролей в Privilegd Identity Management.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: b6e7a9c4a761b699ffe4128a62fd69a75a0662df
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722271"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="74595-103">тип ресурса privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="74595-103">privilegedRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="74595-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74595-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74595-105">Представляет запрос на операции назначения ролей в Privilegd Identity Management.</span><span class="sxs-lookup"><span data-stu-id="74595-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="74595-106">`privilegedRoleAssignmentRequest` — это объект, моделируемый билетами, используемый для управления жизненным циклом назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-106">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="74595-107">Он представляет намерения и решения пользователей и администраторов, а также обеспечивает гибкость, чтобы включить реализацию повторяющихся schduling, ворота утверждения и так далее, по сравнению с непосредственной разоблачения и операций, а также и функций `POST` `LIST` на `MY` `Cancel` `governanceRoleAssignment` .</span><span class="sxs-lookup"><span data-stu-id="74595-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="74595-108">Методы</span><span class="sxs-lookup"><span data-stu-id="74595-108">Methods</span></span>

| <span data-ttu-id="74595-109">Метод</span><span class="sxs-lookup"><span data-stu-id="74595-109">Method</span></span>       | <span data-ttu-id="74595-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74595-110">Return Type</span></span> | <span data-ttu-id="74595-111">Описание</span><span class="sxs-lookup"><span data-stu-id="74595-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="74595-112">Список</span><span class="sxs-lookup"><span data-stu-id="74595-112">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="74595-113">[коллекция privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="74595-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="74595-114">Список запросов на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-114">List role assignment requests.</span></span>|
|[<span data-ttu-id="74595-115">Создание</span><span class="sxs-lookup"><span data-stu-id="74595-115">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="74595-116">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="74595-116">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="74595-117">Создайте запрос для управления жизненным циклом существующего или нового назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-117">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="74595-118">Отмена</span><span class="sxs-lookup"><span data-stu-id="74595-118">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="74595-119">Отмена ожидающих запросов на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-119">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="74595-120">My</span><span class="sxs-lookup"><span data-stu-id="74595-120">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="74595-121">Получите запрос на назначение ролей для текущего requstor.</span><span class="sxs-lookup"><span data-stu-id="74595-121">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="74595-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="74595-122">Properties</span></span>

| <span data-ttu-id="74595-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="74595-123">Property</span></span>     | <span data-ttu-id="74595-124">Тип</span><span class="sxs-lookup"><span data-stu-id="74595-124">Type</span></span>        | <span data-ttu-id="74595-125">Описание</span><span class="sxs-lookup"><span data-stu-id="74595-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74595-126">id</span><span class="sxs-lookup"><span data-stu-id="74595-126">id</span></span>|<span data-ttu-id="74595-127">String</span><span class="sxs-lookup"><span data-stu-id="74595-127">String</span></span>| <span data-ttu-id="74595-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74595-128">Read-only.</span></span> <span data-ttu-id="74595-129">ID запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-129">The id of the role assignment request.</span></span>|
|<span data-ttu-id="74595-130">assignmentState</span><span class="sxs-lookup"><span data-stu-id="74595-130">assignmentState</span></span>|<span data-ttu-id="74595-131">String</span><span class="sxs-lookup"><span data-stu-id="74595-131">String</span></span>| <span data-ttu-id="74595-132">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="74595-132">The state of the assignment.</span></span> <span data-ttu-id="74595-133">Это значение может быть для присвоения, если оно непосредственно назначено администраторами или активировано при назначении, назначенного `Eligible` `Active` `Active` пользователями.</span><span class="sxs-lookup"><span data-stu-id="74595-133">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="74595-134">duration</span><span class="sxs-lookup"><span data-stu-id="74595-134">duration</span></span>|<span data-ttu-id="74595-135">String</span><span class="sxs-lookup"><span data-stu-id="74595-135">String</span></span>| <span data-ttu-id="74595-136">Продолжительность назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-136">The duration of a role assignment.</span></span>|
|<span data-ttu-id="74595-137">reason</span><span class="sxs-lookup"><span data-stu-id="74595-137">reason</span></span>|<span data-ttu-id="74595-138">String</span><span class="sxs-lookup"><span data-stu-id="74595-138">String</span></span>| <span data-ttu-id="74595-139">Причина назначения роли.</span><span class="sxs-lookup"><span data-stu-id="74595-139">The reason for the role assignment.</span></span>|
|<span data-ttu-id="74595-140">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="74595-140">requestedDateTime</span></span>|<span data-ttu-id="74595-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74595-141">DateTimeOffset</span></span>| <span data-ttu-id="74595-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74595-142">Read-only.</span></span> <span data-ttu-id="74595-143">Время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="74595-143">The request create time.</span></span> <span data-ttu-id="74595-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="74595-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="74595-145">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="74595-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="74595-146">roleId</span><span class="sxs-lookup"><span data-stu-id="74595-146">roleId</span></span>|<span data-ttu-id="74595-147">String</span><span class="sxs-lookup"><span data-stu-id="74595-147">String</span></span>| <span data-ttu-id="74595-148">ID роли.</span><span class="sxs-lookup"><span data-stu-id="74595-148">The id of the role.</span></span>|
|<span data-ttu-id="74595-149">schedule</span><span class="sxs-lookup"><span data-stu-id="74595-149">schedule</span></span>|[<span data-ttu-id="74595-150">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="74595-150">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="74595-151">Объект расписания запроса назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-151">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="74595-152">status</span><span class="sxs-lookup"><span data-stu-id="74595-152">status</span></span>|<span data-ttu-id="74595-153">String</span><span class="sxs-lookup"><span data-stu-id="74595-153">String</span></span>| <span data-ttu-id="74595-154">Read-only.The status of the role assignment request.</span><span class="sxs-lookup"><span data-stu-id="74595-154">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="74595-155">Значение может быть `NotStarted` , , , , , , , `Completed` , `RequestedApproval` `Scheduled` `Approved` `ApprovalDenied` `ApprovalAborted` `Cancelling` `Cancelled` `Revoked` `RequestExpired` .</span><span class="sxs-lookup"><span data-stu-id="74595-155">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="74595-156">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="74595-156">ticketNumber</span></span>|<span data-ttu-id="74595-157">String</span><span class="sxs-lookup"><span data-stu-id="74595-157">String</span></span>| <span data-ttu-id="74595-158">TicketNumber для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="74595-158">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="74595-159">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="74595-159">ticketSystem</span></span>|<span data-ttu-id="74595-160">String</span><span class="sxs-lookup"><span data-stu-id="74595-160">String</span></span>| <span data-ttu-id="74595-161">TicketSystem для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-161">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="74595-162">type</span><span class="sxs-lookup"><span data-stu-id="74595-162">type</span></span>|<span data-ttu-id="74595-163">String</span><span class="sxs-lookup"><span data-stu-id="74595-163">String</span></span>| <span data-ttu-id="74595-164">Представление типа операции при назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-164">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="74595-165">Значение может `AdminAdd` быть: Администраторы добавляют пользователей в роли; `UserAdd` : Пользователи добавляют назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-165">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="74595-166">userId</span><span class="sxs-lookup"><span data-stu-id="74595-166">userId</span></span>|<span data-ttu-id="74595-167">String</span><span class="sxs-lookup"><span data-stu-id="74595-167">String</span></span>| <span data-ttu-id="74595-168">ID пользователя.</span><span class="sxs-lookup"><span data-stu-id="74595-168">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74595-169">Связи</span><span class="sxs-lookup"><span data-stu-id="74595-169">Relationships</span></span>
| <span data-ttu-id="74595-170">Связь</span><span class="sxs-lookup"><span data-stu-id="74595-170">Relationship</span></span> | <span data-ttu-id="74595-171">Тип</span><span class="sxs-lookup"><span data-stu-id="74595-171">Type</span></span>        | <span data-ttu-id="74595-172">Описание</span><span class="sxs-lookup"><span data-stu-id="74595-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74595-173">roleInfo</span><span class="sxs-lookup"><span data-stu-id="74595-173">roleInfo</span></span>|[<span data-ttu-id="74595-174">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="74595-174">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="74595-175">Объект roleInfo запроса назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="74595-175">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74595-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74595-176">JSON representation</span></span>

<span data-ttu-id="74595-177">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74595-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}-->

```json
{
  "assignmentState": "String",
  "duration": "String",
  "id": "String (identifier)",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleId": "String",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": "String",
  "ticketNumber": "String",
  "ticketSystem": "String",
  "type": "String",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


