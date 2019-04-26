---
title: Тип ресурса Привилежедролеассигнментрекуест
description: Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.
localization_priority: Normal
ms.openlocfilehash: c0e0bbfa76b7ffb4e122d381d45dd4092f0843c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563361"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="5d0b5-103">Тип ресурса Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="5d0b5-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d0b5-104">Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="5d0b5-105">`privilegedRoleAssignmentRequest`— Это объект с моделированием билетов, используемый для управления жизненным циклом назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="5d0b5-106">Он представляет намерение/решение для пользователей и администраторов, а также обеспечивает гибкость, позволяющую включать реализацию перечисленных счдулинг, шлюзов утверждения и т. д., в отличие от прямого предоставления `POST` и `LIST` операций, а также `MY` и `Cancel` функции On `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="5d0b5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5d0b5-107">Methods</span></span>

| <span data-ttu-id="5d0b5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5d0b5-108">Method</span></span>       | <span data-ttu-id="5d0b5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5d0b5-109">Return Type</span></span> | <span data-ttu-id="5d0b5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5d0b5-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="5d0b5-111">List</span><span class="sxs-lookup"><span data-stu-id="5d0b5-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="5d0b5-112">Коллекция [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="5d0b5-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="5d0b5-113">Список запросов на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="5d0b5-114">Создание</span><span class="sxs-lookup"><span data-stu-id="5d0b5-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="5d0b5-115">привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="5d0b5-115">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="5d0b5-116">Создание запроса на управление жизненным циклом существующего или нового назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="5d0b5-117">Отмена</span><span class="sxs-lookup"><span data-stu-id="5d0b5-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="5d0b5-118">Отмена ожидающего запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="5d0b5-119">My</span><span class="sxs-lookup"><span data-stu-id="5d0b5-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="5d0b5-120">Получение запроса на назначение роли для текущего рекустор.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-120">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="5d0b5-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d0b5-121">Properties</span></span>

| <span data-ttu-id="5d0b5-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d0b5-122">Property</span></span>     | <span data-ttu-id="5d0b5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5d0b5-123">Type</span></span>        | <span data-ttu-id="5d0b5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5d0b5-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d0b5-125">id</span><span class="sxs-lookup"><span data-stu-id="5d0b5-125">id</span></span>|<span data-ttu-id="5d0b5-126">String</span><span class="sxs-lookup"><span data-stu-id="5d0b5-126">String</span></span>| <span data-ttu-id="5d0b5-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-127">Read-only.</span></span> <span data-ttu-id="5d0b5-128">Идентификатор запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="5d0b5-129">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="5d0b5-129">assignmentState</span></span>|<span data-ttu-id="5d0b5-130">String</span><span class="sxs-lookup"><span data-stu-id="5d0b5-130">String</span></span>| <span data-ttu-id="5d0b5-131">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-131">The state of the assignment.</span></span> <span data-ttu-id="5d0b5-132">Значение может быть `Eligible` для правого назначения `Active` , если оно напрямую назначено `Active` администраторами или активировано в соответствии с подходящими пользователями.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="5d0b5-133">duration</span><span class="sxs-lookup"><span data-stu-id="5d0b5-133">duration</span></span>|<span data-ttu-id="5d0b5-134">String</span><span class="sxs-lookup"><span data-stu-id="5d0b5-134">String</span></span>| <span data-ttu-id="5d0b5-135">Продолжительность назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="5d0b5-136">причиной</span><span class="sxs-lookup"><span data-stu-id="5d0b5-136">reason</span></span>|<span data-ttu-id="5d0b5-137">String</span><span class="sxs-lookup"><span data-stu-id="5d0b5-137">String</span></span>| <span data-ttu-id="5d0b5-138">Причина назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="5d0b5-139">Рекуестеддатетиме</span><span class="sxs-lookup"><span data-stu-id="5d0b5-139">requestedDateTime</span></span>|<span data-ttu-id="5d0b5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d0b5-140">DateTimeOffset</span></span>| <span data-ttu-id="5d0b5-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-141">Read-only.</span></span> <span data-ttu-id="5d0b5-142">Время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-142">The request create time.</span></span> <span data-ttu-id="5d0b5-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5d0b5-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5d0b5-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5d0b5-145">roleId</span><span class="sxs-lookup"><span data-stu-id="5d0b5-145">roleId</span></span>|<span data-ttu-id="5d0b5-146">String</span><span class="sxs-lookup"><span data-stu-id="5d0b5-146">String</span></span>| <span data-ttu-id="5d0b5-147">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-147">The id of the role.</span></span>|
|<span data-ttu-id="5d0b5-148">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="5d0b5-148">schedule</span></span>|[<span data-ttu-id="5d0b5-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="5d0b5-149">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="5d0b5-150">Объект расписания для запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="5d0b5-151">status</span><span class="sxs-lookup"><span data-stu-id="5d0b5-151">status</span></span>|<span data-ttu-id="5d0b5-152">Строка</span><span class="sxs-lookup"><span data-stu-id="5d0b5-152">String</span></span>| <span data-ttu-id="5d0b5-153">Только для чтения. состояние запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="5d0b5-154">Возможные значения `NotStarted``Completed`:,`RequestedApproval``Scheduled``Approved``Revoked``RequestExpired`,,,,,,,,,.`ApprovalDenied``ApprovalAborted``Cancelling``Cancelled`</span><span class="sxs-lookup"><span data-stu-id="5d0b5-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="5d0b5-155">Тиккетнумбер</span><span class="sxs-lookup"><span data-stu-id="5d0b5-155">ticketNumber</span></span>|<span data-ttu-id="5d0b5-156">String</span><span class="sxs-lookup"><span data-stu-id="5d0b5-156">String</span></span>| <span data-ttu-id="5d0b5-157">Тиккетнумбер для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="5d0b5-158">Тиккетсистем</span><span class="sxs-lookup"><span data-stu-id="5d0b5-158">ticketSystem</span></span>|<span data-ttu-id="5d0b5-159">String</span><span class="sxs-lookup"><span data-stu-id="5d0b5-159">String</span></span>| <span data-ttu-id="5d0b5-160">Тиккетсистем для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="5d0b5-161">type</span><span class="sxs-lookup"><span data-stu-id="5d0b5-161">type</span></span>|<span data-ttu-id="5d0b5-162">String</span><span class="sxs-lookup"><span data-stu-id="5d0b5-162">String</span></span>| <span data-ttu-id="5d0b5-163">Представляет тип операции для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-163">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="5d0b5-164">Возможные значения `AdminAdd`: Администраторы Add Users to Roles; `UserAdd`: Пользователи добавляют назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="5d0b5-165">userId</span><span class="sxs-lookup"><span data-stu-id="5d0b5-165">userId</span></span>|<span data-ttu-id="5d0b5-166">String</span><span class="sxs-lookup"><span data-stu-id="5d0b5-166">String</span></span>| <span data-ttu-id="5d0b5-167">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d0b5-168">Связи</span><span class="sxs-lookup"><span data-stu-id="5d0b5-168">Relationships</span></span>
| <span data-ttu-id="5d0b5-169">Отношение</span><span class="sxs-lookup"><span data-stu-id="5d0b5-169">Relationship</span></span> | <span data-ttu-id="5d0b5-170">Тип</span><span class="sxs-lookup"><span data-stu-id="5d0b5-170">Type</span></span>        | <span data-ttu-id="5d0b5-171">Описание</span><span class="sxs-lookup"><span data-stu-id="5d0b5-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d0b5-172">Ролеинфо</span><span class="sxs-lookup"><span data-stu-id="5d0b5-172">roleInfo</span></span>|[<span data-ttu-id="5d0b5-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="5d0b5-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="5d0b5-174">Объект Ролеинфо запроса назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d0b5-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d0b5-175">JSON representation</span></span>

<span data-ttu-id="5d0b5-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d0b5-176">The following is a JSON representation of the resource.</span></span>

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
