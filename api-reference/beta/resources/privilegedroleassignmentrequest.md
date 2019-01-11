---
title: Тип ресурса privilegedRoleAssignmentRequest
description: Представляет запрос для операций назначения роли управления удостоверениями Privilegd.
localization_priority: Normal
ms.openlocfilehash: bfe3b6802136b2848f36abef08134efd0eb82518
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880131"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="8caac-103">Тип ресурса privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8caac-103">privilegedRoleAssignmentRequest resource type</span></span>

> <span data-ttu-id="8caac-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8caac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8caac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8caac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8caac-106">Представляет запрос для операций назначения роли управления удостоверениями Privilegd.</span><span class="sxs-lookup"><span data-stu-id="8caac-106">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="8caac-107">`privilegedRoleAssignmentRequest`смоделировать билетов сущности, используется для управления жизненным циклом назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8caac-107">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="8caac-108">Он представляет намерения/решение для пользователей и администраторов, а также обеспечивает гибкость для внедрения повторяющаяся schduling, шлюзы утверждения и т. д. по сравнению с непосредственно предоставление `POST` и `LIST` операции в том числе в `MY` и `Cancel` функции на `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="8caac-108">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="8caac-109">Методы</span><span class="sxs-lookup"><span data-stu-id="8caac-109">Methods</span></span>

| <span data-ttu-id="8caac-110">Метод</span><span class="sxs-lookup"><span data-stu-id="8caac-110">Method</span></span>       | <span data-ttu-id="8caac-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8caac-111">Return Type</span></span> | <span data-ttu-id="8caac-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8caac-112">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="8caac-113">List</span><span class="sxs-lookup"><span data-stu-id="8caac-113">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="8caac-114">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8caac-114">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="8caac-115">Список запросов назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8caac-115">List role assignment requests.</span></span>|
|<span data-ttu-id="8caac-116">[создание](../api/privilegedroleassignmentrequest-post.md);</span><span class="sxs-lookup"><span data-stu-id="8caac-116">[Create](../api/privilegedroleassignmentrequest-post.md)</span></span>|  [<span data-ttu-id="8caac-117">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="8caac-117">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="8caac-118">Создание запроса для управления жизненным циклом существующего или нового назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8caac-118">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="8caac-119">Отмена</span><span class="sxs-lookup"><span data-stu-id="8caac-119">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="8caac-120">Отмена назначения запроса ожидающие роли.</span><span class="sxs-lookup"><span data-stu-id="8caac-120">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="8caac-121">My</span><span class="sxs-lookup"><span data-stu-id="8caac-121">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="8caac-122">Получите запрос назначения ролей для текущего requstor.</span><span class="sxs-lookup"><span data-stu-id="8caac-122">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="8caac-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="8caac-123">Properties</span></span>

| <span data-ttu-id="8caac-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="8caac-124">Property</span></span>     | <span data-ttu-id="8caac-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8caac-125">Type</span></span>        | <span data-ttu-id="8caac-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8caac-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8caac-127">id</span><span class="sxs-lookup"><span data-stu-id="8caac-127">id</span></span>|<span data-ttu-id="8caac-128">Строка</span><span class="sxs-lookup"><span data-stu-id="8caac-128">String</span></span>| <span data-ttu-id="8caac-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8caac-129">Read-only.</span></span> <span data-ttu-id="8caac-130">Идентификатор запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="8caac-130">The id of the role assignment request.</span></span>|
|<span data-ttu-id="8caac-131">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8caac-131">assignmentState</span></span>|<span data-ttu-id="8caac-132">Строка</span><span class="sxs-lookup"><span data-stu-id="8caac-132">String</span></span>| <span data-ttu-id="8caac-133">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="8caac-133">The state of the assignment.</span></span> <span data-ttu-id="8caac-134">Значение может быть `Eligible` подходящими назначения `Active` - если она назначена непосредственно `Active` администраторами, или активируемого на допустимость назначения для пользователей.</span><span class="sxs-lookup"><span data-stu-id="8caac-134">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="8caac-135">duration</span><span class="sxs-lookup"><span data-stu-id="8caac-135">duration</span></span>|<span data-ttu-id="8caac-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8caac-136">String</span></span>| <span data-ttu-id="8caac-137">Длительность назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8caac-137">The duration of a role assignment.</span></span>|
|<span data-ttu-id="8caac-138">Причина</span><span class="sxs-lookup"><span data-stu-id="8caac-138">reason</span></span>|<span data-ttu-id="8caac-139">Строка</span><span class="sxs-lookup"><span data-stu-id="8caac-139">String</span></span>| <span data-ttu-id="8caac-140">Причина для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8caac-140">The reason for the role assignment.</span></span>|
|<span data-ttu-id="8caac-141">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="8caac-141">requestedDateTime</span></span>|<span data-ttu-id="8caac-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8caac-142">DateTimeOffset</span></span>| <span data-ttu-id="8caac-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8caac-143">Read-only.</span></span> <span data-ttu-id="8caac-144">Время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="8caac-144">The request create time.</span></span> <span data-ttu-id="8caac-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8caac-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8caac-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8caac-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8caac-147">roleId</span><span class="sxs-lookup"><span data-stu-id="8caac-147">roleId</span></span>|<span data-ttu-id="8caac-148">Строка</span><span class="sxs-lookup"><span data-stu-id="8caac-148">String</span></span>| <span data-ttu-id="8caac-149">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="8caac-149">The id of the role.</span></span>|
|<span data-ttu-id="8caac-150">расписание</span><span class="sxs-lookup"><span data-stu-id="8caac-150">schedule</span></span>|[<span data-ttu-id="8caac-151">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8caac-151">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="8caac-152">Объект расписание запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8caac-152">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="8caac-153">status</span><span class="sxs-lookup"><span data-stu-id="8caac-153">status</span></span>|<span data-ttu-id="8caac-154">Строка</span><span class="sxs-lookup"><span data-stu-id="8caac-154">String</span></span>| <span data-ttu-id="8caac-155">Состояние чтения only.The запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8caac-155">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="8caac-156">Значение может быть `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="8caac-156">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="8caac-157">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="8caac-157">ticketNumber</span></span>|<span data-ttu-id="8caac-158">Строка</span><span class="sxs-lookup"><span data-stu-id="8caac-158">String</span></span>| <span data-ttu-id="8caac-159">TicketNumber назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8caac-159">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="8caac-160">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="8caac-160">ticketSystem</span></span>|<span data-ttu-id="8caac-161">Строка</span><span class="sxs-lookup"><span data-stu-id="8caac-161">String</span></span>| <span data-ttu-id="8caac-162">TicketSystem назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8caac-162">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="8caac-163">type</span><span class="sxs-lookup"><span data-stu-id="8caac-163">type</span></span>|<span data-ttu-id="8caac-164">Строка</span><span class="sxs-lookup"><span data-stu-id="8caac-164">String</span></span>| <span data-ttu-id="8caac-165">Представляет тип операции в назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="8caac-165">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="8caac-166">Значение может быть `AdminAdd`: администраторам Добавление пользователей в роли. `UserAdd`: Добавление назначений ролей пользователей.</span><span class="sxs-lookup"><span data-stu-id="8caac-166">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="8caac-167">userId</span><span class="sxs-lookup"><span data-stu-id="8caac-167">userId</span></span>|<span data-ttu-id="8caac-168">String</span><span class="sxs-lookup"><span data-stu-id="8caac-168">String</span></span>| <span data-ttu-id="8caac-169">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="8caac-169">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8caac-170">Связи</span><span class="sxs-lookup"><span data-stu-id="8caac-170">Relationships</span></span>
| <span data-ttu-id="8caac-171">Связь</span><span class="sxs-lookup"><span data-stu-id="8caac-171">Relationship</span></span> | <span data-ttu-id="8caac-172">Тип</span><span class="sxs-lookup"><span data-stu-id="8caac-172">Type</span></span>        | <span data-ttu-id="8caac-173">Описание</span><span class="sxs-lookup"><span data-stu-id="8caac-173">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8caac-174">roleInfo</span><span class="sxs-lookup"><span data-stu-id="8caac-174">roleInfo</span></span>|[<span data-ttu-id="8caac-175">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="8caac-175">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="8caac-176">Объект roleInfo запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8caac-176">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8caac-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8caac-177">JSON representation</span></span>

<span data-ttu-id="8caac-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8caac-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
