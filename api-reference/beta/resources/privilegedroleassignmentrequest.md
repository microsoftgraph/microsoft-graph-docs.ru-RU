---
title: Тип ресурса Привилежедролеассигнментрекуест
description: Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: c9ca647c7d2af82f76348fa737d15995d8a2ed96
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217899"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="3bbcd-103">Тип ресурса Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="3bbcd-103">privilegedRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="3bbcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bbcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bbcd-105">Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="3bbcd-106">`privilegedRoleAssignmentRequest`— Это объект с моделированием билетов, используемый для управления жизненным циклом назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-106">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="3bbcd-107">Он представляет намерение/решение для пользователей и администраторов, а также обеспечивает гибкость, позволяющую включать реализацию перечисленных счдулинг, шлюзов утверждения и т. `POST` д `LIST` `MY` `Cancel` `governanceRoleAssignment`., как и в сравнении с прямым предоставлением и работой, а также функциями.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="3bbcd-108">Методы</span><span class="sxs-lookup"><span data-stu-id="3bbcd-108">Methods</span></span>

| <span data-ttu-id="3bbcd-109">Метод</span><span class="sxs-lookup"><span data-stu-id="3bbcd-109">Method</span></span>       | <span data-ttu-id="3bbcd-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3bbcd-110">Return Type</span></span> | <span data-ttu-id="3bbcd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3bbcd-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="3bbcd-112">List</span><span class="sxs-lookup"><span data-stu-id="3bbcd-112">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="3bbcd-113">Коллекция [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="3bbcd-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="3bbcd-114">Список запросов на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-114">List role assignment requests.</span></span>|
|<span data-ttu-id="3bbcd-115">[создание](../api/privilegedroleassignmentrequest-post.md);</span><span class="sxs-lookup"><span data-stu-id="3bbcd-115">[Create](../api/privilegedroleassignmentrequest-post.md)</span></span>|  [<span data-ttu-id="3bbcd-116">привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="3bbcd-116">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="3bbcd-117">Создание запроса на управление жизненным циклом существующего или нового назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-117">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="3bbcd-118">Отмена</span><span class="sxs-lookup"><span data-stu-id="3bbcd-118">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="3bbcd-119">Отмена ожидающего запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-119">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="3bbcd-120">My</span><span class="sxs-lookup"><span data-stu-id="3bbcd-120">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="3bbcd-121">Получение запроса на назначение роли для текущего рекустор.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-121">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="3bbcd-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="3bbcd-122">Properties</span></span>

| <span data-ttu-id="3bbcd-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="3bbcd-123">Property</span></span>     | <span data-ttu-id="3bbcd-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3bbcd-124">Type</span></span>        | <span data-ttu-id="3bbcd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3bbcd-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3bbcd-126">id</span><span class="sxs-lookup"><span data-stu-id="3bbcd-126">id</span></span>|<span data-ttu-id="3bbcd-127">Строка</span><span class="sxs-lookup"><span data-stu-id="3bbcd-127">String</span></span>| <span data-ttu-id="3bbcd-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-128">Read-only.</span></span> <span data-ttu-id="3bbcd-129">Идентификатор запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-129">The id of the role assignment request.</span></span>|
|<span data-ttu-id="3bbcd-130">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="3bbcd-130">assignmentState</span></span>|<span data-ttu-id="3bbcd-131">Строка</span><span class="sxs-lookup"><span data-stu-id="3bbcd-131">String</span></span>| <span data-ttu-id="3bbcd-132">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-132">The state of the assignment.</span></span> <span data-ttu-id="3bbcd-133">Значение может быть `Eligible` для правого назначения `Active` , если оно напрямую назначено `Active` администраторами или активировано в соответствии с подходящими пользователями.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-133">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="3bbcd-134">duration</span><span class="sxs-lookup"><span data-stu-id="3bbcd-134">duration</span></span>|<span data-ttu-id="3bbcd-135">Строка</span><span class="sxs-lookup"><span data-stu-id="3bbcd-135">String</span></span>| <span data-ttu-id="3bbcd-136">Продолжительность назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-136">The duration of a role assignment.</span></span>|
|<span data-ttu-id="3bbcd-137">reason</span><span class="sxs-lookup"><span data-stu-id="3bbcd-137">reason</span></span>|<span data-ttu-id="3bbcd-138">Строка</span><span class="sxs-lookup"><span data-stu-id="3bbcd-138">String</span></span>| <span data-ttu-id="3bbcd-139">Причина назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-139">The reason for the role assignment.</span></span>|
|<span data-ttu-id="3bbcd-140">рекуестеддатетиме</span><span class="sxs-lookup"><span data-stu-id="3bbcd-140">requestedDateTime</span></span>|<span data-ttu-id="3bbcd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bbcd-141">DateTimeOffset</span></span>| <span data-ttu-id="3bbcd-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-142">Read-only.</span></span> <span data-ttu-id="3bbcd-143">Время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-143">The request create time.</span></span> <span data-ttu-id="3bbcd-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3bbcd-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3bbcd-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3bbcd-146">roleId</span><span class="sxs-lookup"><span data-stu-id="3bbcd-146">roleId</span></span>|<span data-ttu-id="3bbcd-147">Строка</span><span class="sxs-lookup"><span data-stu-id="3bbcd-147">String</span></span>| <span data-ttu-id="3bbcd-148">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-148">The id of the role.</span></span>|
|<span data-ttu-id="3bbcd-149">schedule</span><span class="sxs-lookup"><span data-stu-id="3bbcd-149">schedule</span></span>|[<span data-ttu-id="3bbcd-150">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3bbcd-150">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="3bbcd-151">Объект расписания для запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-151">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="3bbcd-152">status</span><span class="sxs-lookup"><span data-stu-id="3bbcd-152">status</span></span>|<span data-ttu-id="3bbcd-153">String</span><span class="sxs-lookup"><span data-stu-id="3bbcd-153">String</span></span>| <span data-ttu-id="3bbcd-154">Только для чтения. состояние запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-154">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="3bbcd-155">Возможные значения `NotStarted``Completed`:,`RequestedApproval``Scheduled``Approved``Revoked``RequestExpired`,,,,,,,,,.`ApprovalDenied``ApprovalAborted``Cancelling``Cancelled`</span><span class="sxs-lookup"><span data-stu-id="3bbcd-155">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="3bbcd-156">тиккетнумбер</span><span class="sxs-lookup"><span data-stu-id="3bbcd-156">ticketNumber</span></span>|<span data-ttu-id="3bbcd-157">Строка</span><span class="sxs-lookup"><span data-stu-id="3bbcd-157">String</span></span>| <span data-ttu-id="3bbcd-158">Тиккетнумбер для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-158">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="3bbcd-159">тиккетсистем</span><span class="sxs-lookup"><span data-stu-id="3bbcd-159">ticketSystem</span></span>|<span data-ttu-id="3bbcd-160">Строка</span><span class="sxs-lookup"><span data-stu-id="3bbcd-160">String</span></span>| <span data-ttu-id="3bbcd-161">Тиккетсистем для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-161">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="3bbcd-162">type</span><span class="sxs-lookup"><span data-stu-id="3bbcd-162">type</span></span>|<span data-ttu-id="3bbcd-163">Строка</span><span class="sxs-lookup"><span data-stu-id="3bbcd-163">String</span></span>| <span data-ttu-id="3bbcd-164">Представляет тип операции для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-164">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="3bbcd-165">Возможные значения `AdminAdd`: администраторы добавляют пользователей к ролям; `UserAdd`: Пользователи добавляют назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-165">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="3bbcd-166">userId</span><span class="sxs-lookup"><span data-stu-id="3bbcd-166">userId</span></span>|<span data-ttu-id="3bbcd-167">String</span><span class="sxs-lookup"><span data-stu-id="3bbcd-167">String</span></span>| <span data-ttu-id="3bbcd-168">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-168">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bbcd-169">Отношения</span><span class="sxs-lookup"><span data-stu-id="3bbcd-169">Relationships</span></span>
| <span data-ttu-id="3bbcd-170">Связь</span><span class="sxs-lookup"><span data-stu-id="3bbcd-170">Relationship</span></span> | <span data-ttu-id="3bbcd-171">Тип</span><span class="sxs-lookup"><span data-stu-id="3bbcd-171">Type</span></span>        | <span data-ttu-id="3bbcd-172">Описание</span><span class="sxs-lookup"><span data-stu-id="3bbcd-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3bbcd-173">ролеинфо</span><span class="sxs-lookup"><span data-stu-id="3bbcd-173">roleInfo</span></span>|[<span data-ttu-id="3bbcd-174">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="3bbcd-174">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="3bbcd-175">Объект Ролеинфо запроса назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-175">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bbcd-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3bbcd-176">JSON representation</span></span>

<span data-ttu-id="3bbcd-177">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-177">The following is a JSON representation of the resource.</span></span>

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
