---
title: Тип ресурса privilegedRoleAssignmentRequest
description: Представляет запрос для операций назначения роли управления удостоверениями Privilegd.
localization_priority: Normal
ms.openlocfilehash: a0cb0bc03d8bb2436e45139bc9db5322cc3970cf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571751"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="7d70b-103">Тип ресурса privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7d70b-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d70b-104">Представляет запрос для операций назначения роли управления удостоверениями Privilegd.</span><span class="sxs-lookup"><span data-stu-id="7d70b-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="7d70b-105">`privilegedRoleAssignmentRequest`смоделировать билетов сущности, используется для управления жизненным циклом назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="7d70b-106">Он представляет намерения/решение для пользователей и администраторов, а также обеспечивает гибкость для внедрения повторяющаяся schduling, шлюзы утверждения и т. д. по сравнению с непосредственно предоставление `POST` и `LIST` операции в том числе в `MY` и `Cancel` функции на `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="7d70b-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="7d70b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7d70b-107">Methods</span></span>

| <span data-ttu-id="7d70b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7d70b-108">Method</span></span>       | <span data-ttu-id="7d70b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7d70b-109">Return Type</span></span> | <span data-ttu-id="7d70b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7d70b-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="7d70b-111">List</span><span class="sxs-lookup"><span data-stu-id="7d70b-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="7d70b-112">[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7d70b-112">[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="7d70b-113">Список запросов назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="7d70b-114">Create</span><span class="sxs-lookup"><span data-stu-id="7d70b-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="7d70b-115">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7d70b-115">privilegedRoleAssignmentRequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="7d70b-116">Создание запроса для управления жизненным циклом существующего или нового назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7d70b-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="7d70b-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="7d70b-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="7d70b-118">Отмена назначения запроса ожидающие роли.</span><span class="sxs-lookup"><span data-stu-id="7d70b-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="7d70b-119">My</span><span class="sxs-lookup"><span data-stu-id="7d70b-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="7d70b-120">Получите запрос назначения ролей для текущего запрашивающего.</span><span class="sxs-lookup"><span data-stu-id="7d70b-120">Get role assignment request for current requestor.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d70b-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d70b-121">Properties</span></span>

| <span data-ttu-id="7d70b-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d70b-122">Property</span></span>     | <span data-ttu-id="7d70b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7d70b-123">Type</span></span>        | <span data-ttu-id="7d70b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7d70b-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7d70b-125">id</span><span class="sxs-lookup"><span data-stu-id="7d70b-125">id</span></span>|<span data-ttu-id="7d70b-126">Строка</span><span class="sxs-lookup"><span data-stu-id="7d70b-126">String</span></span>| <span data-ttu-id="7d70b-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d70b-127">Read-only.</span></span> <span data-ttu-id="7d70b-128">Идентификатор запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="7d70b-129">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7d70b-129">assignmentState</span></span>|<span data-ttu-id="7d70b-130">Строка</span><span class="sxs-lookup"><span data-stu-id="7d70b-130">String</span></span>| <span data-ttu-id="7d70b-131">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="7d70b-131">The state of the assignment.</span></span> <span data-ttu-id="7d70b-132">Значение может быть `Eligible` подходящими назначения `Active` - если она назначена непосредственно `Active` администраторами, или активируемого на допустимость назначения для пользователей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="7d70b-133">duration</span><span class="sxs-lookup"><span data-stu-id="7d70b-133">duration</span></span>|<span data-ttu-id="7d70b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7d70b-134">String</span></span>| <span data-ttu-id="7d70b-135">Длительность назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="7d70b-136">Причина</span><span class="sxs-lookup"><span data-stu-id="7d70b-136">reason</span></span>|<span data-ttu-id="7d70b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7d70b-137">String</span></span>| <span data-ttu-id="7d70b-138">Причина для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="7d70b-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d70b-139">requestedDateTime</span></span>|<span data-ttu-id="7d70b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d70b-140">DateTimeOffset</span></span>| <span data-ttu-id="7d70b-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d70b-141">Read-only.</span></span> <span data-ttu-id="7d70b-142">Время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="7d70b-142">The request create time.</span></span> <span data-ttu-id="7d70b-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7d70b-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d70b-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7d70b-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7d70b-145">roleId</span><span class="sxs-lookup"><span data-stu-id="7d70b-145">roleId</span></span>|<span data-ttu-id="7d70b-146">Строка</span><span class="sxs-lookup"><span data-stu-id="7d70b-146">String</span></span>| <span data-ttu-id="7d70b-147">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="7d70b-147">The id of the role.</span></span>|
|<span data-ttu-id="7d70b-148">расписание</span><span class="sxs-lookup"><span data-stu-id="7d70b-148">schedule</span></span>|[<span data-ttu-id="7d70b-149">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7d70b-149"> microsoft.graph.governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="7d70b-150">Объект расписание запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="7d70b-151">status</span><span class="sxs-lookup"><span data-stu-id="7d70b-151">status</span></span>|<span data-ttu-id="7d70b-152">Строка</span><span class="sxs-lookup"><span data-stu-id="7d70b-152">String</span></span>| <span data-ttu-id="7d70b-153">Состояние чтения only.The запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="7d70b-154">Значение может быть `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="7d70b-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="7d70b-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="7d70b-155">ticketNumber</span></span>|<span data-ttu-id="7d70b-156">Строка</span><span class="sxs-lookup"><span data-stu-id="7d70b-156">String</span></span>| <span data-ttu-id="7d70b-157">TicketNumber назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7d70b-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="7d70b-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="7d70b-158">ticketSystem</span></span>|<span data-ttu-id="7d70b-159">Строка</span><span class="sxs-lookup"><span data-stu-id="7d70b-159">String</span></span>| <span data-ttu-id="7d70b-160">TicketSystem назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7d70b-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="7d70b-161">type</span><span class="sxs-lookup"><span data-stu-id="7d70b-161">type</span></span>|<span data-ttu-id="7d70b-162">Строка</span><span class="sxs-lookup"><span data-stu-id="7d70b-162">String</span></span>| <span data-ttu-id="7d70b-163">Представляет тип операции в назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-163">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="7d70b-164">Значение может быть `AdminAdd`: администраторам Добавление пользователей в роли. `UserAdd`: Добавление назначений ролей пользователей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="7d70b-165">userId</span><span class="sxs-lookup"><span data-stu-id="7d70b-165">userId</span></span>|<span data-ttu-id="7d70b-166">String</span><span class="sxs-lookup"><span data-stu-id="7d70b-166">String</span></span>| <span data-ttu-id="7d70b-167">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="7d70b-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d70b-168">Связи</span><span class="sxs-lookup"><span data-stu-id="7d70b-168">Relationships</span></span>
| <span data-ttu-id="7d70b-169">Связь</span><span class="sxs-lookup"><span data-stu-id="7d70b-169">Relationship</span></span> | <span data-ttu-id="7d70b-170">Тип</span><span class="sxs-lookup"><span data-stu-id="7d70b-170">Type</span></span>        | <span data-ttu-id="7d70b-171">Описание</span><span class="sxs-lookup"><span data-stu-id="7d70b-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7d70b-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="7d70b-172">roleInfo</span></span>|[<span data-ttu-id="7d70b-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="7d70b-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="7d70b-174">Объект roleInfo запрос назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="7d70b-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d70b-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d70b-175">JSON representation</span></span>

<span data-ttu-id="7d70b-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d70b-176">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
