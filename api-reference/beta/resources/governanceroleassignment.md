---
title: тип ресурса governanceRoleAssignment
description: Представляет назначение пользователя или группы роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 532ea3c1d8fe5b1bc1128994c96c493774e9b19b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964571"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="29f23-103">тип ресурса governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="29f23-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="29f23-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="29f23-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="29f23-105">Представляет назначение пользователя или группы роли.</span><span class="sxs-lookup"><span data-stu-id="29f23-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="29f23-106">Привилегированное управление удостоверениями (PIM) поддерживает два типа назначений:</span><span class="sxs-lookup"><span data-stu-id="29f23-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="29f23-107">Активное назначение — представляет прямой или активированный доступ к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="29f23-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="29f23-108">Право назначения — представляет промежуточный этап привилегированного доступа к ресурсам между отсутствием доступа и прямым доступом.</span><span class="sxs-lookup"><span data-stu-id="29f23-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="29f23-109">Администраторы могут назначать пользователям или группам заранее, и всякий раз, когда необходим доступ, необходимо получить мгновенный доступ к ресурсу `eligible assignment` `activation` в течение нескольких `eligible assignment` часов.</span><span class="sxs-lookup"><span data-stu-id="29f23-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="29f23-110">После активации будет создано для пользователей или членов группы, чтобы указать `active assignment` активированный статус.</span><span class="sxs-lookup"><span data-stu-id="29f23-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="29f23-111">Методы</span><span class="sxs-lookup"><span data-stu-id="29f23-111">Methods</span></span>

| <span data-ttu-id="29f23-112">Метод</span><span class="sxs-lookup"><span data-stu-id="29f23-112">Method</span></span>          | <span data-ttu-id="29f23-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="29f23-113">Return Type</span></span> |<span data-ttu-id="29f23-114">Описание</span><span class="sxs-lookup"><span data-stu-id="29f23-114">Description</span></span>|
|:------------|:--------|:--------|
|<span data-ttu-id="29f23-115">[получение](../api/governanceroleassignment-get.md);</span><span class="sxs-lookup"><span data-stu-id="29f23-115">[Get](../api/governanceroleassignment-get.md)</span></span> |  [<span data-ttu-id="29f23-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="29f23-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="29f23-117">Чтение свойств и связей объекта назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="29f23-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="29f23-118">List</span><span class="sxs-lookup"><span data-stu-id="29f23-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="29f23-119">[коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="29f23-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="29f23-120">Список набор назначений ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="29f23-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="29f23-121">Экспорт</span><span class="sxs-lookup"><span data-stu-id="29f23-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="29f23-122">octet-stream</span><span class="sxs-lookup"><span data-stu-id="29f23-122">octet-stream</span></span> |<span data-ttu-id="29f23-123">Скачайте коллекцию назначений ролей на ресурсе и сохраните в качестве `.csv` файла.</span><span class="sxs-lookup"><span data-stu-id="29f23-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="29f23-124">Нет `POST` , или операции `PUT` `PATCH` `DELETE` поддерживаются в `roleAssignments` наборе сущности.</span><span class="sxs-lookup"><span data-stu-id="29f23-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="29f23-125">Любые операции по созданию, обновлению и удаляемой работе `governanceRoleAssignment` делаются `governanceRoleAssignmentRequest` путем .</span><span class="sxs-lookup"><span data-stu-id="29f23-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="29f23-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="29f23-126">Properties</span></span>
| <span data-ttu-id="29f23-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="29f23-127">Property</span></span>  | <span data-ttu-id="29f23-128">Тип</span><span class="sxs-lookup"><span data-stu-id="29f23-128">Type</span></span>      |<span data-ttu-id="29f23-129">Описание</span><span class="sxs-lookup"><span data-stu-id="29f23-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="29f23-130">id</span><span class="sxs-lookup"><span data-stu-id="29f23-130">id</span></span>         |<span data-ttu-id="29f23-131">Строка</span><span class="sxs-lookup"><span data-stu-id="29f23-131">String</span></span>     |<span data-ttu-id="29f23-132">ID назначения роли.</span><span class="sxs-lookup"><span data-stu-id="29f23-132">The ID of the role assignment.</span></span> <span data-ttu-id="29f23-133">Он находится в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="29f23-133">It is in GUID format.</span></span>|
|<span data-ttu-id="29f23-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="29f23-134">resourceId</span></span> |<span data-ttu-id="29f23-135">String</span><span class="sxs-lookup"><span data-stu-id="29f23-135">String</span></span>     |<span data-ttu-id="29f23-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29f23-136">Required.</span></span> <span data-ttu-id="29f23-137">ID ресурса, с которым связано назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="29f23-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="29f23-138">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="29f23-138">roleDefinitionId</span></span>|<span data-ttu-id="29f23-139">Строка</span><span class="sxs-lookup"><span data-stu-id="29f23-139">String</span></span>|<span data-ttu-id="29f23-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29f23-140">Required.</span></span> <span data-ttu-id="29f23-141">ID определения роли, с которым связано назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="29f23-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="29f23-142">subjectId</span><span class="sxs-lookup"><span data-stu-id="29f23-142">subjectId</span></span>|<span data-ttu-id="29f23-143">Строка</span><span class="sxs-lookup"><span data-stu-id="29f23-143">String</span></span>       |<span data-ttu-id="29f23-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29f23-144">Required.</span></span> <span data-ttu-id="29f23-145">ID субъекта, с которым связано назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="29f23-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="29f23-146">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="29f23-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="29f23-147">Строка</span><span class="sxs-lookup"><span data-stu-id="29f23-147">String</span></span>|<span data-ttu-id="29f23-148">Если это и создано из-за активации `active assignment` на , он представляет собой `eligible assignment` ID `eligible assignment` этого; В противном случае значение `null` .</span><span class="sxs-lookup"><span data-stu-id="29f23-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="29f23-149">externalId</span><span class="sxs-lookup"><span data-stu-id="29f23-149">externalId</span></span>   |<span data-ttu-id="29f23-150">String</span><span class="sxs-lookup"><span data-stu-id="29f23-150">String</span></span>     |<span data-ttu-id="29f23-151">Внешний ID ресурса, который используется для определения назначения роли в поставщике.</span><span class="sxs-lookup"><span data-stu-id="29f23-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="29f23-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="29f23-152">startDateTime</span></span>|<span data-ttu-id="29f23-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29f23-153">DateTimeOffset</span></span>|<span data-ttu-id="29f23-154">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="29f23-154">The start time of the role assignment.</span></span> <span data-ttu-id="29f23-155">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="29f23-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29f23-156">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="29f23-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="29f23-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="29f23-157">endDateTime</span></span>|<span data-ttu-id="29f23-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29f23-158">DateTimeOffset</span></span>|<span data-ttu-id="29f23-159">Для назначения непостоянных ролей это время, когда срок действия назначения роли истекает.</span><span class="sxs-lookup"><span data-stu-id="29f23-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="29f23-160">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="29f23-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29f23-161">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="29f23-161">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="29f23-162">assignmentState</span><span class="sxs-lookup"><span data-stu-id="29f23-162">assignmentState</span></span>|<span data-ttu-id="29f23-163">Строка</span><span class="sxs-lookup"><span data-stu-id="29f23-163">String</span></span>  |<span data-ttu-id="29f23-164">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="29f23-164">The state of the assignment.</span></span> <span data-ttu-id="29f23-165">Это значение может быть для назначения, назначенного администраторами, или если оно непосредственно назначено администраторами или активировано при назначении, назначенное `Eligible` `Active` `Active` пользователями.</span><span class="sxs-lookup"><span data-stu-id="29f23-165">The value can be `Eligible` for eligible assignment or `Active` if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="29f23-166">memberType</span><span class="sxs-lookup"><span data-stu-id="29f23-166">memberType</span></span>|<span data-ttu-id="29f23-167">Строка</span><span class="sxs-lookup"><span data-stu-id="29f23-167">String</span></span>      |<span data-ttu-id="29f23-168">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="29f23-168">The type of member.</span></span> <span data-ttu-id="29f23-169">Значение может быть: (если назначение роли наследуется из области родительского ресурса), (если назначение роли не наследуется, а происходит от членства в групповом назначении) или (если назначение роли не наследуется или не от группового `Inherited` `Group` `User` назначения).</span><span class="sxs-lookup"><span data-stu-id="29f23-169">The value can be: `Inherited` (if the role assignment is inherited from a parent resource scope), `Group` (if the role assignment is not inherited, but comes from the membership of a group assignment), or `User` (if the role assignment is neither inherited nor from a group assignment).</span></span>|


## <a name="relationships"></a><span data-ttu-id="29f23-170">Связи</span><span class="sxs-lookup"><span data-stu-id="29f23-170">Relationships</span></span>
| <span data-ttu-id="29f23-171">Связь</span><span class="sxs-lookup"><span data-stu-id="29f23-171">Relationship</span></span> | <span data-ttu-id="29f23-172">Тип</span><span class="sxs-lookup"><span data-stu-id="29f23-172">Type</span></span>   |<span data-ttu-id="29f23-173">Описание</span><span class="sxs-lookup"><span data-stu-id="29f23-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29f23-174">resource</span><span class="sxs-lookup"><span data-stu-id="29f23-174">resource</span></span>|[<span data-ttu-id="29f23-175">governanceResource</span><span class="sxs-lookup"><span data-stu-id="29f23-175">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="29f23-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29f23-176">Read-only.</span></span> <span data-ttu-id="29f23-177">Ресурс, связанный с назначением ролей.</span><span class="sxs-lookup"><span data-stu-id="29f23-177">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="29f23-178">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="29f23-178">roleDefinition</span></span>|[<span data-ttu-id="29f23-179">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="29f23-179">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="29f23-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29f23-180">Read-only.</span></span> <span data-ttu-id="29f23-181">Определение роли, связанное с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="29f23-181">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="29f23-182">subject</span><span class="sxs-lookup"><span data-stu-id="29f23-182">subject</span></span>|[<span data-ttu-id="29f23-183">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="29f23-183">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="29f23-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29f23-184">Read-only.</span></span> <span data-ttu-id="29f23-185">Тема, связанная с назначением ролей.</span><span class="sxs-lookup"><span data-stu-id="29f23-185">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="29f23-186">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="29f23-186">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="29f23-187">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="29f23-187">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="29f23-188">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29f23-188">Read-only.</span></span> <span data-ttu-id="29f23-189">Если это и `active assignment` создается из-за активации на объекте, он представляет `eligible assignment` объект `eligible assignment` этого; В противном случае значение `null` .</span><span class="sxs-lookup"><span data-stu-id="29f23-189">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="29f23-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29f23-190">JSON representation</span></span>

<span data-ttu-id="29f23-191">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29f23-191">Here is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


