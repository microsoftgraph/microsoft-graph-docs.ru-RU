---
title: Тип ресурса Привилежедролеассигнментрекуест
description: Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.
localization_priority: Normal
ms.openlocfilehash: 240c84ecb0bf4f8d0e171f647f21eb6730c28d44
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621216"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="8702d-103">Тип ресурса Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="8702d-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8702d-104">Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="8702d-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="8702d-105">`privilegedRoleAssignmentRequest`— Это объект с моделированием билетов, используемый для управления жизненным циклом назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="8702d-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="8702d-106">Он представляет намерение/решение для пользователей и администраторов, а также обеспечивает гибкость, позволяющую включать реализацию перечисленных счдулинг, шлюзов утверждения и т. д., в отличие от прямого предоставления `POST` и `LIST` операций, а также `MY` и `Cancel` функции On `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="8702d-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="8702d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8702d-107">Methods</span></span>

| <span data-ttu-id="8702d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8702d-108">Method</span></span>       | <span data-ttu-id="8702d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8702d-109">Return Type</span></span> | <span data-ttu-id="8702d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8702d-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="8702d-111">List</span><span class="sxs-lookup"><span data-stu-id="8702d-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="8702d-112">Коллекция [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8702d-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="8702d-113">Список запросов на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="8702d-113">List role assignment requests.</span></span>|
|<span data-ttu-id="8702d-114">[создание](../api/privilegedroleassignmentrequest-post.md);</span><span class="sxs-lookup"><span data-stu-id="8702d-114">[Create](../api/privilegedroleassignmentrequest-post.md)</span></span>|  [<span data-ttu-id="8702d-115">привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="8702d-115">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="8702d-116">Создание запроса на управление жизненным циклом существующего или нового назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="8702d-117">Отмена</span><span class="sxs-lookup"><span data-stu-id="8702d-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="8702d-118">Отмена ожидающего запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="8702d-119">My</span><span class="sxs-lookup"><span data-stu-id="8702d-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="8702d-120">Получение запроса на назначение роли для текущего рекустор.</span><span class="sxs-lookup"><span data-stu-id="8702d-120">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="8702d-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="8702d-121">Properties</span></span>

| <span data-ttu-id="8702d-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="8702d-122">Property</span></span>     | <span data-ttu-id="8702d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8702d-123">Type</span></span>        | <span data-ttu-id="8702d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8702d-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8702d-125">id</span><span class="sxs-lookup"><span data-stu-id="8702d-125">id</span></span>|<span data-ttu-id="8702d-126">String</span><span class="sxs-lookup"><span data-stu-id="8702d-126">String</span></span>| <span data-ttu-id="8702d-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8702d-127">Read-only.</span></span> <span data-ttu-id="8702d-128">Идентификатор запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="8702d-129">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="8702d-129">assignmentState</span></span>|<span data-ttu-id="8702d-130">String</span><span class="sxs-lookup"><span data-stu-id="8702d-130">String</span></span>| <span data-ttu-id="8702d-131">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="8702d-131">The state of the assignment.</span></span> <span data-ttu-id="8702d-132">Значение может быть `Eligible` для правого назначения `Active` , если оно напрямую назначено `Active` администраторами или активировано в соответствии с подходящими пользователями.</span><span class="sxs-lookup"><span data-stu-id="8702d-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="8702d-133">duration</span><span class="sxs-lookup"><span data-stu-id="8702d-133">duration</span></span>|<span data-ttu-id="8702d-134">String</span><span class="sxs-lookup"><span data-stu-id="8702d-134">String</span></span>| <span data-ttu-id="8702d-135">Продолжительность назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="8702d-136">причиной</span><span class="sxs-lookup"><span data-stu-id="8702d-136">reason</span></span>|<span data-ttu-id="8702d-137">String</span><span class="sxs-lookup"><span data-stu-id="8702d-137">String</span></span>| <span data-ttu-id="8702d-138">Причина назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="8702d-139">Рекуестеддатетиме</span><span class="sxs-lookup"><span data-stu-id="8702d-139">requestedDateTime</span></span>|<span data-ttu-id="8702d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8702d-140">DateTimeOffset</span></span>| <span data-ttu-id="8702d-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8702d-141">Read-only.</span></span> <span data-ttu-id="8702d-142">Время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="8702d-142">The request create time.</span></span> <span data-ttu-id="8702d-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8702d-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8702d-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8702d-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8702d-145">roleId</span><span class="sxs-lookup"><span data-stu-id="8702d-145">roleId</span></span>|<span data-ttu-id="8702d-146">String</span><span class="sxs-lookup"><span data-stu-id="8702d-146">String</span></span>| <span data-ttu-id="8702d-147">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-147">The id of the role.</span></span>|
|<span data-ttu-id="8702d-148">schedule</span><span class="sxs-lookup"><span data-stu-id="8702d-148">schedule</span></span>|[<span data-ttu-id="8702d-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8702d-149">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="8702d-150">Объект расписания для запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="8702d-151">status</span><span class="sxs-lookup"><span data-stu-id="8702d-151">status</span></span>|<span data-ttu-id="8702d-152">String</span><span class="sxs-lookup"><span data-stu-id="8702d-152">String</span></span>| <span data-ttu-id="8702d-153">Только для чтения. состояние запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="8702d-154">Возможные значения `NotStarted``Completed`:,`RequestedApproval``Scheduled``Approved``Revoked``RequestExpired`,,,,,,,,,.`ApprovalDenied``ApprovalAborted``Cancelling``Cancelled`</span><span class="sxs-lookup"><span data-stu-id="8702d-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="8702d-155">Тиккетнумбер</span><span class="sxs-lookup"><span data-stu-id="8702d-155">ticketNumber</span></span>|<span data-ttu-id="8702d-156">String</span><span class="sxs-lookup"><span data-stu-id="8702d-156">String</span></span>| <span data-ttu-id="8702d-157">Тиккетнумбер для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="8702d-158">Тиккетсистем</span><span class="sxs-lookup"><span data-stu-id="8702d-158">ticketSystem</span></span>|<span data-ttu-id="8702d-159">String</span><span class="sxs-lookup"><span data-stu-id="8702d-159">String</span></span>| <span data-ttu-id="8702d-160">Тиккетсистем для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="8702d-161">type</span><span class="sxs-lookup"><span data-stu-id="8702d-161">type</span></span>|<span data-ttu-id="8702d-162">String</span><span class="sxs-lookup"><span data-stu-id="8702d-162">String</span></span>| <span data-ttu-id="8702d-163">Представляет тип операции для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-163">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="8702d-164">Возможные значения `AdminAdd`: Администраторы Add Users to Roles; `UserAdd`: Пользователи добавляют назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8702d-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="8702d-165">userId</span><span class="sxs-lookup"><span data-stu-id="8702d-165">userId</span></span>|<span data-ttu-id="8702d-166">String</span><span class="sxs-lookup"><span data-stu-id="8702d-166">String</span></span>| <span data-ttu-id="8702d-167">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="8702d-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8702d-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="8702d-168">Relationships</span></span>
| <span data-ttu-id="8702d-169">Отношение</span><span class="sxs-lookup"><span data-stu-id="8702d-169">Relationship</span></span> | <span data-ttu-id="8702d-170">Тип</span><span class="sxs-lookup"><span data-stu-id="8702d-170">Type</span></span>        | <span data-ttu-id="8702d-171">Описание</span><span class="sxs-lookup"><span data-stu-id="8702d-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8702d-172">Ролеинфо</span><span class="sxs-lookup"><span data-stu-id="8702d-172">roleInfo</span></span>|[<span data-ttu-id="8702d-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="8702d-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="8702d-174">Объект Ролеинфо запроса назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8702d-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8702d-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8702d-175">JSON representation</span></span>

<span data-ttu-id="8702d-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8702d-176">The following is a JSON representation of the resource.</span></span>

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
